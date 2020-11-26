<template>
  <div class="login">
    <form action class="form">
      <label class="form-label1">Inicio de sesión</label>
      <label class="form-label">Correo:</label>
      <input class="form-input" type="text" id="ruc" required placeholder="Correo" v-model="email">
      <label class="form-label">Contraseña:</label>
      <input class="form-input" type="password" id="password" placeholder="Contraseña" v-model="password">
      <input class="form-submit" type="button" id="login" value="Login" @click="searchEmail()">
      <p class="passMessage" v-if="this.status === 2 ">Contraseña equivocada</p>
    </form>
  </div>
</template>

<script>
    import CustomerDataService from "@/services/CustomersDataService";

    export default {
        name: "Login",
        data() {
            return {
                email: "",
                password:"",
                currentIndex: "",
                originalPassword: "",
                status: 0,
            };
        },
        methods: {
            searchEmail() {
                CustomerDataService.findByEmail(this.email)
                .then(response => {
                    console.log(response.data[0]["password"])
                    console.log(this.password)
                    this.status = 2;
                    if(this.password === response.data[0]["password"]) {
                        this.status = 1;
                        console.log(this.status)
                        console.log(response.data[0]["id"])
                        if(this.status === 1) {
                          this.currentTutorial = response.data[0];
                          document.location.href = `/customer-profile/${response.data[0]["id"]}`;
                        }
                    }

                })
                .catch(e => {
                    console.log(e);
                });
            }
        },
        mounted() {
            this.retrieveTutorials();
            var input = document.getElementById("password");
            input.addEventListener("keyup", function(event) {
            // Number 13 is the "Enter" key on the keyboard
            if (event.keyCode === 13) {
              // Cancel the default action, if needed
              event.preventDefault();
              // Trigger the button element with a click
              document.getElementById("login").click();
            }
          });
        }
    }
</script>

<style scoped>
.login {
  padding: 2rem;
  margin-left: 200px;
}

.form {
  margin: 3rem auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 20%;
  min-width: 350px;
  max-width: 100%;
  background: rgba(19, 35, 47, 0.9);
  border-radius: 5px;
  padding: 40px;
  box-shadow: 0 4px 10px 4px rgba(0, 0, 0, 0.3);
}
.form-label {
  margin-top: 2rem;
  color: white;
  margin-bottom: 0.5rem;
}
.form-label1{
  color: white;
  font-size: 30px;
}
.form-input {
  padding: 10px 15px;
  background: none;
  background-image: none;
  border: 1px solid white;
  color: white;
}
.form-submit {
  background: #1ab188;
  border: none;
  color: white;
  margin-top: 3rem;
  padding: 1rem 0;
  cursor: pointer;
  transition: background 0.2s;
}
.passMessage {
  margin-top: 10px;
  color: #ff0000;;
  font-size: 20px;
}
</style>
