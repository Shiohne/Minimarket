<template>
<div>
<vue-custom-scrollbar class="scroll-area"  :settings="settings" @ps-scroll-y="scrollHanle">

      <p> Se incluirán los siguientes artículos definidos por la Superintendencia de Banca y Seguros del Perú (SBS),
        para sentar bases más claras en el sustento de la funcionalidad de la aplicación.
         Resolución S.B.S N° 8181 - 2012
         Ley Nº 28587: Ley complementaria a la Ley de protección al consumidor en materia de servicios financieros
      </p>
      <p>
         Artículo 3°. - Principio de transparencia de información
         Las empresas deberán ser plenamente transparentes en la difusión, aplicación y modificación de las
         condiciones contractuales, tasas de interés compensatorio, tasas de interés moratorio o penalidades
         aplicables en caso de incumplimiento, comisiones y gastos asociados a las operaciones activas y pasivas
         que realicen, así como a los servicios que brinden, según corresponda.
         La transparencia de información es un mecanismo que busca mejorar el acceso a la información de los
         usuarios. En ese sentido, las empresas deberán ser diligentes en las explicaciones que brindan respecto a
         los productos y servicios ofrecidos, con el fin de que los usuarios comprendan sus características,
         beneficios, riesgos y condiciones aplicables y puedan, de manera responsable, tomar decisiones de consumo
         informadas.
      </p>
      <p>
         Artículo 4°. - Determinación de las tasas de interés
         Las empresas, de conformidad con lo dispuesto en el artículo 9° de la Ley General, pueden determinar
         libremente las tasas de interés compensatorio y moratorio para sus operaciones activas y pasivas,
         considerando para tal efecto lo indicado en el artículo 5° de la ley Complementaria.
         Las tasas de interés compensatorio y moratorio deben ser expresadas en forma efectiva anual, debiéndose
         considerar para tal efecto que se trata de un año de trescientos sesenta (360) días. Para su
         determinación y aplicación, las empresas deberán tener en cuenta la regulación que sobre la materia emite
         el Banco Central de Reserva del Perú con acuerdo a su Ley Orgánica.
      </p>
      <p>
         Artículo 6°. - Tasa de costo efectivo anual
         La tasa de costo efectivo anual (TCEA) es aquella que permite igualar el valor actual de todas las cuotas
         con el monto que efectivamente haya sido recibido en préstamo. Para este cálculo se incluirán las cuotas
         que involucran el principal, intereses, comisiones y gastos, que de acuerdo con lo pactado serán
         trasladados al cliente, incluidos los seguros en los casos que se trate de créditos de consumo y/o
         hipotecarios para vivienda. No se incluirán en este cálculo aquellos pagos por servicios provistos por
         terceros que directamente sean pagados por el cliente, ni los tributos que resulten aplicables.

         Los cálculos de la TCEA, para el caso de las operaciones activas bajo el sistema de cuotas, procederán
         bajo el supuesto de cumplimiento de todas las condiciones pactadas, utilizando la fórmula señalada en el
         Anexo N° 1 del Reglamento.

         Los cálculos de la TCEA para el caso de operaciones activas bajo el sistema revolvente, atendiendo a sus
         características, corresponden a un patrón estandarizado de comparación de costos y procederán bajo el
         supuesto de cumplimiento de todas las condiciones pactadas, de acuerdo con lo indicado en el Anexo N° 1-A
         del Reglamento.
      </p>
     <p>
       Artículo 9°. -Definición de comisiones y gastos
       Las comisiones y gastos se determinarán libremente de conformidad con lo establecido en el artículo 9° de la
       Ley General: a) Las comisiones son retribuciones por operaciones o servicios adicionales y/o complementarios a
       las operaciones contratadas por los usuarios, que hayan sido previamente acordados y efectivamente prestados
       por la empresa. b) Los gastos son costos por operaciones o servicios adicionales y/o complementarios a las
       operaciones contratadas, debidamente acreditados en que incurre la empresa con terceros por cuenta del usuario
       que pueden ser trasladados al cliente, en caso así se establezca expresamente en los contratos respectivos.
     </p>
      <p>
         Artículo 11°.- Sustento de comisiones y gastos

         Las comisiones o gastos deben implicar la prestación de un servicio efectivo, tener justificación técnica
         e implicar un costo real y demostrable para el proveedor del servicio.

         Las empresas deberán tener a disposición de la Superintendencia, el sustento técnico y económico de las
         comisiones y gastos que cobren, en los términos que se señale para tal efecto.
         La exigencia de justificación técnica y económica tiene por finalidad sustentar que las comisiones
         correspondan a servicios efectivamente prestados en tanto que los gastos correspondan
         a costos reales en los que se ha incurrido con terceros. En el caso de los gastos, el sustento de costos
         debe justificar el monto que se consigna como tal concepto.
      </p>
     <p>
       Artículo 22°. -Pago anticipado y adelanto de cuotas
       22.1 Los usuarios tienen derecho a efectuar pagos por encima de la cuota exigible en el periodo, considerando
       para tal efecto lo siguiente:
       a. No deben establecerse condiciones o limitaciones para el ejercicio del derecho.
       b. No pueden aplicarse comisiones, gastos, penalidades de ningún tipo por el ejercicio del derecho o cobros
       de naturaleza o efecto similar.
       c. Debe informarse, al momento de efectuar la operación, del monto que resulta aplicable por concepto de
       impuestos. Los usuarios podrán efectuar los pagos en cualquiera de las oficinas de atención al público de la
       empresa en las que puedan realizarse operaciones de pagos y desembolsos, así como en otros canales adicionales
       puestos a disposición por la empresa y que sean informados a los usuarios.
       d. Los usuarios podrán efectuar los pagos en cualquiera de las oficinas de atención al público de la empresa en
       las que puedan realizarse operaciones de pagos y desembolsos, así como en otros canales adicionales puestos a
       disposición por la empresa y que sean informados a los usuarios.
     </p>
           <p>
         Artículo 24°.- Modificación de las tasas de interés
         Las empresas deberán informar a sus clientes la modificación de las tasas de interés en contratos
         distintos a los créditos a plazo fijo o depósitos a plazo fijo, en forma previa cuando se trate de
         incrementos en el caso de las operaciones activas y reducciones en el caso de las operaciones pasivas. La
         respectiva comunicación deberá ser efectuada con una anticipación no menor a cuarenta y cinco (45) días
         indicando la fecha o el momento, a partir del cual, la modificación entrará en vigencia
      </p>
     <p>
       Artículo 30°. -Reglas aplicables para el incremento de la línea de crédito
       Los incrementos de la línea de crédito no podrán efectuarse a través de modificaciones unilaterales por parte de
       las empresas. En ese sentido, no corresponde efectuar un aviso previo conforme lo señala el artículo 26° del
       Reglamento, sino que deberá requerirse el consentimiento expreso del cliente en cada oportunidad en que este se
       realice, a través de los mecanismos que para tal efecto pacten las partes, dejando constancia expresa de la
       fecha a partir de la cual se procederá a realizar el aumento de la línea de crédito. No podrá considerarse el
       silencio del cliente como señal de aceptación.
     </p>
    </vue-custom-scrollbar>
  </div>
</template>

<script>
import vueCustomScrollbar from 'vue-custom-scrollbar'
import "vue-custom-scrollbar/dist/vueScrollbar.css"
export default {
  components: {
    vueCustomScrollbar
  },
  data() {
    return {
      settings: {
        suppressScrollY: false,
        suppressScrollX: false,
        wheelPropagation: false
      }
    }
  },
  methods: {
    scrollHanle(evt) {
      console.log(evt)
    }
  }
}
</script>
<style >
.scroll-area {
  padding: 20px;
  border-color: #ffa504;
  background-color: #f5f5f5;
  position: relative;
  margin-left: 140px;
  margin-top: 80px;
  width: 1200px;
  height: 690px;
}
</style>
