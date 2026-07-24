<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
     

      #Actividad_Cuestionario
      <ActividadController :cuestionario="cuestionario"/>
  
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Nombre del CF',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> identificar la importancia de las fases de la venta, el rol de la comunicación y el impacto del <i><i>merchandising</i></i> en el fortalecimiento de la relación con el cliente.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO.',
      preguntas: [
        {
          id: 1,
          texto: '¿Qué es la venta?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Una actividad exclusiva de publicidad.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Un proceso estructurado de interacción con el cliente para satisfacer necesidades y generar intercambios.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Un sistema de distribución de productos.',
              esCorrecta: false,
            },
            { id: 'd', texto: 'Una estrategia financiera.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 2,
          texto: '¿Cuál es el principal objetivo de una venta?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reducir costos de producción.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'Incrementar inventarios.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'Satisfacer necesidades del cliente mediante un intercambio de valor.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Eliminar la competencia.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 3,
          texto: '¿Qué elemento es fundamental durante el proceso de venta?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ignorar las necesidades del cliente.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'Reducir la comunicación.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Aumentar los precios constantemente.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Mantener una interacción efectiva con el cliente.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 4,
          texto: '¿Qué papel cumple la comunicación en las ventas?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Facilitar la transmisión de información y la persuasión del cliente.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Controlar los costos operativos.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Diseñar productos nuevos.', esCorrecta: false },
            { id: 'd', texto: 'Administrar inventarios.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 5,
          texto:
            '¿Por qué se considera la comunicación un eje fundamental en las ventas?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Porque reemplaza al producto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Porque permite transmitir mensajes claros y persuadir al cliente.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Porque elimina la competencia.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Porque incrementa automáticamente las ganancias.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 6,
          texto: '¿Qué característica debe tener una comunicación efectiva?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Ser confusa y extensa.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Ser exclusivamente escrita.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Ser clara, precisa y comprensible.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Ser compleja y técnica.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 7,
          texto: '¿Cuál de los siguientes es un medio de comunicación?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Inventario.', esCorrecta: false },
            { id: 'b', texto: 'Factura.', esCorrecta: false },
            { id: 'c', texto: 'Cotización.', esCorrecta: false },
            { id: 'd', texto: 'Correo electrónico.', esCorrecta: true },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 8,
          texto: '¿Qué se busca lograr mediante la comunicación comercial?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Incrementar los costos.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Reducir la atención al cliente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Informar, persuadir y fortalecer la relación con el cliente.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Limitar las ventas.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 9,
          texto: '¿Qué es el <i>merchandising</i>?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Una técnica de producción.', esCorrecta: false },
            { id: 'b', texto: 'Un proceso de fabricación.', esCorrecta: false },
            {
              id: 'c',
              texto:
                'Una estrategia para influir en la decisión de compra en el punto de venta.',
              esCorrecta: true,
            },
            { id: 'd', texto: 'Un sistema de transporte.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 10,
          texto: '¿Cuál es el objetivo principal del <i>merchandising</i>?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reducir la cantidad de productos.',
              esCorrecta: false,
            },
            { id: 'b', texto: 'Eliminar la publicidad.', esCorrecta: false },
            { id: 'c', texto: 'Disminuir las ventas.', esCorrecta: false },
            {
              id: 'd',
              texto:
                'Estimular la compra de productos por parte del consumidor.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 11,
          texto: '¿Dónde se aplica principalmente el <i>merchandising</i>?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'En el punto de venta.', esCorrecta: true },
            { id: 'b', texto: 'En las fábricas.', esCorrecta: false },
            {
              id: 'c',
              texto: 'En las entidades financieras.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'En los centros de distribución.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 12,
          texto: '¿Cuál es una herramienta común del <i>merchandising</i>?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Estados financieros.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Exhibición estratégica de productos.',
              esCorrecta: true,
            },
            { id: 'c', texto: 'Nómina de empleados.', esCorrecta: false },
            { id: 'd', texto: 'Manual de funciones.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 13,
          texto: '¿Qué efecto puede generar una buena exhibición de productos?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Confusión en el consumidor.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Disminución de la visibilidad.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Mayor interés y probabilidad de compra.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Menor rotación de inventarios.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 14,
          texto: '¿Qué habilidad es importante para un vendedor?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Falta de escucha.', esCorrecta: false },
            { id: 'b', texto: 'Desinterés por el cliente.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Capacidad de comunicación y persuasión.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Evitar el contacto con los clientes.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 15,
          texto:
            '¿Qué ocurre cuando la venta, la comunicación y el <i>merchandising</i> trabajan de manera integrada?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Se incrementan los errores operativos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Se genera una mejor experiencia para el consumidor y mejores resultados para la empresa.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Disminuyen las oportunidades de venta.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Se reducen los canales de comunicación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 16,
          texto:
            '¿Qué beneficio aporta una comunicación clara durante la venta?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Aumenta los malentendidos.', esCorrecta: false },
            {
              id: 'b',
              texto: 'Reduce la confianza del cliente.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Dificulta la negociación.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Facilita la comprensión de la oferta comercial.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 17,
          texto:
            '¿Cuál de los siguientes medios corresponde a una comunicación digital?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Cartel físico.', esCorrecta: false },
            { id: 'b', texto: 'Volante impreso.', esCorrecta: false },
            { id: 'c', texto: 'Redes sociales.', esCorrecta: true },
            { id: 'd', texto: 'Valla publicitaria.', esCorrecta: false },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 18,
          texto:
            '¿Qué busca la persuasión dentro de la comunicación comercial?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Influir de manera positiva en la decisión de compra del cliente.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Obligar al cliente a comprar.',
              esCorrecta: false,
            },
            { id: 'c', texto: 'Incrementar los precios.', esCorrecta: false },
            {
              id: 'd',
              texto: 'Limitar las opciones de compra.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 19,
          texto:
            '¿Qué característica debe tener un mensaje comercial efectivo?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            { id: 'a', texto: 'Ser ambiguo.', esCorrecta: false },
            { id: 'b', texto: 'Ser excesivamente técnico.', esCorrecta: false },
            {
              id: 'c',
              texto: 'Ser difícil de interpretar.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Ser claro, atractivo y relevante para el cliente.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
        {
          id: 20,
          texto:
            '¿Cuál es el resultado esperado de una estrategia adecuada de ventas y comunicación?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Menor satisfacción del cliente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Disminución de la fidelización.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Incremento de las ventas y fortalecimiento de las relaciones con los clientes.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Reducción de la competitividad.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia un adecuado dominio de los fundamentos de las Ventas, comunicación y <i>merchandising</i>.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente los contenidos del componente formativo Ventas, comunicación y <i>merchandising</i>.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
