<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
  
      #Actividad                
        <Actividad :cuestionario="cuestionario"/>
  
  </template>

<script>
import Actividad from 'ecored-pkg-fliz/plugin/components/actividad/Actividad.vue'
export default {
  name: 'ActividadDidactica',
  components: {
    Actividad,
  },
  data: () => ({
    cuestionario: {
      tema: 'Recepción y registro de requerimientos del cliente',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> evaluar la capacidad para identificar, registrar y gestionar adecuadamente los requerimientos del cliente mediante el uso de sistemas de información, bases de datos y elaboración de informes que fortalezcan la relación organizacional.',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!.',
      titulo_reprobado: 'VUELVA A INTENTARLO.',
      preguntas: [
        {
          id: 1,
          texto:
            '¿Cuál es una función principal de la organización empresarial?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Definir una estructura para coordinar actividades y responsabilidades.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Eliminar todos los niveles de responsabilidad de la empresa.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Evitar que las áreas de la empresa compartan información.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Reemplazar las necesidades de los clientes por decisiones internas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'La organización empresarial estructura las actividades y responsabilidades para orientar el funcionamiento de la empresa.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 2,
          texto:
            '¿Qué propósito cumplen los sistemas de información en una organización?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Almacenar únicamente documentos impresos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Apoyar la gestión mediante la captura, procesamiento y disponibilidad de información.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'Impedir que los colaboradores consulten datos necesarios para su labor.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Sustituir todos los procedimientos de atención al cliente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Los sistemas de información ayudan a gestionar y procesar datos para que estén disponibles cuando se necesitan.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 3,
          texto: '¿Qué significa la sigla CRM en el contexto empresarial?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Control de Recursos de Manufactura.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Centro de Registro de Mercancías.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Customer Relationship Management, gestión de relaciones con los clientes.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Consulta de Reportes Mensuales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'CRM corresponde a Customer Relationship Management y permite consolidar información e interacciones de los clientes.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 4,
          texto:
            '¿Qué utilidad tiene un sistema CRM para un agente de servicio?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Consultar información del cliente y sus interacciones con la empresa.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Modificar sin restricciones cualquier dato financiero de la organización.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Evitar que se registren las solicitudes de los clientes.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Reemplazar la comunicación entre el agente y el cliente.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'El CRM reúne información del cliente y sus interacciones, lo que facilita una atención más empática y asertiva.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 5,
          texto:
            'En una base de datos relacional, ¿cómo se pueden vincular dos tablas?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Mediante colores y formatos de celda.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'A través de campos que tienen información relacionada en común.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Únicamente mediante archivos impresos.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Eliminando los identificadores de cada tabla.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Las bases de datos relacionales permiten relacionar tablas mediante campos que establecen correspondencias entre los datos.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 6,
          texto: '¿Qué describe mejor un perfil de acceso a una base de datos?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'El diseño visual de la pantalla de inicio.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'La cantidad de clientes que visita una sede.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Las operaciones que un usuario puede realizar según su rol.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'La lista de productos que ofrece la empresa.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Los perfiles asocian a cada rol las operaciones específicas que el usuario está autorizado a realizar.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 7,
          texto:
            '¿Cuál de las siguientes acciones contribuye a la seguridad de la información?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Permitir que todos los usuarios tengan los mismos permisos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Evitar la actualización de los registros.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Compartir las credenciales de acceso entre los colaboradores.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Controlar los accesos y procurar la disponibilidad y actualización de los datos.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'La seguridad de la información implica proteger los datos y gestionar su acceso, disponibilidad y actualización.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 8,
          texto: 'En servicio al cliente, ¿qué se entiende por requerimiento?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Una solicitud que realiza el cliente a través de un canal oficial habilitado por la empresa.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Una instrucción interna que nunca se comunica al cliente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Un informe financiero elaborado exclusivamente por la gerencia.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Una campaña publicitaria diseñada para captar nuevos usuarios.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'El requerimiento es una solicitud del cliente recibida mediante un canal oficial de la organización.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 9,
          texto:
            '¿Cuál de estas situaciones corresponde a un requerimiento informativo?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Solicitar que se corrija una factura con un cobro incorrecto.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Consultar el horario de atención de una sucursal.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Reportar una falla en la conexión a internet.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Presentar una queja por el trato recibido.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Las consultas sobre horarios, direcciones, precios y características de productos son requerimientos informativos.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 10,
          texto: '¿Qué significan las letras PQRSF?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Productos, calidad, registros, sistemas y facturas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Procesos, quejas, reportes, servicios y formatos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Peticiones, quejas, reclamos, sugerencias y felicitaciones.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Peticiones, consultas, respuestas, solicitudes y facturación.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'PQRSF corresponde a peticiones, quejas, reclamos, sugerencias y felicitaciones.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 11,
          texto:
            '¿Cuál es la diferencia entre una queja y una sugerencia en la gestión de PQRSF?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'La queja siempre es una felicitación y la sugerencia siempre es una solicitud de pago.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'No existe ninguna diferencia entre ambas.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La sugerencia comunica una inconformidad y la queja reconoce un buen servicio.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'La queja expresa inconformidad, mientras que la sugerencia propone una mejora.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'La queja comunica inconformidad o dificultad; la sugerencia plantea una propuesta de mejora.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 12,
          texto:
            '¿Cuál de estas situaciones corresponde a un requerimiento de soporte técnico?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Preguntar por la dirección de una sede.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Informar que el servicio de internet no funciona.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Felicitar a un colaborador por su atención.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Consultar las características de un producto.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Reportar que un servicio no funciona corresponde a una necesidad de soporte técnico.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 13,
          texto:
            '¿Qué debe hacer el agente después de recibir y validar un requerimiento, de acuerdo con el procedimiento de la empresa?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Registrar el caso y comunicar al cliente la información pertinente sobre su gestión.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Cerrar el caso sin informar al cliente.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Compartir los datos del cliente con personas ajenas al proceso.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Prometer una solución sin revisar el alcance ni el procedimiento.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'El registro y la comunicación del estado del caso favorecen la trazabilidad y la claridad en la atención.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 14,
          texto:
            '¿Qué implica la inclusión durante la recepción de requerimientos?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Aplicar una única forma de atención sin considerar diferencias.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Atender solamente a clientes que usan canales digitales.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Considerar y valorar las particularidades, necesidades y estilos de las personas.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto: 'Evitar que el cliente explique sus necesidades.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'La inclusión implica considerar las particularidades y necesidades de las personas durante la interacción.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 15,
          texto:
            '¿En qué situación puede surgir una objeción durante la atención?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Cuando el cliente ya recibió toda la información y no tiene dudas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Cuando el cliente siente que el agente no comprende su solicitud o necesita más explicación.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Únicamente cuando el cliente felicita a la empresa.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Cuando el agente elabora un informe mensual sin interacción con clientes.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Las objeciones pueden aparecer cuando el cliente siente que no se comprende su solicitud o requiere aclaraciones.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 16,
          texto:
            '¿Cuál es una respuesta adecuada ante una objeción del cliente?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Interrumpirlo para terminar rápidamente la conversación.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Desestimar sus dudas porque el procedimiento ya está definido.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Discutir con el cliente para demostrar que está equivocado.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Escuchar su inquietud, aclarar la información y responder con empatía y asertividad.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'La escucha, la empatía y la comunicación asertiva ayudan a comprender y gestionar las objeciones.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 17,
          texto:
            '¿Para qué se utilizan principalmente los informes empresariales?',
          imagen: require('@/assets/actividad/imagen5.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Resumir la planeación, gestión o seguimiento de un tema, actividad o proyecto.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Reemplazar todos los registros de las bases de datos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Evitar la comunicación de resultados a los responsables.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Presentar únicamente opiniones sin relación con la información recopilada.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Los informes permiten resumir y comunicar información sobre la planeación, gestión o seguimiento de un asunto.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 18,
          texto: '¿Qué caracteriza a un informe expositivo?',
          imagen: require('@/assets/actividad/imagen5.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Busca principalmente convencer al lector para que apruebe una propuesta.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Plantea una hipótesis y demuestra obligatoriamente una postura personal.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Describe hechos o actividades sin profundizar necesariamente en el análisis.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Se limita a presentar recomendaciones sin exponer información.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'El informe expositivo presenta información descriptiva sobre hechos o actividades y no requiere profundizar en el análisis.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 19,
          texto:
            '¿Qué diferencia a un informe interpretativo de uno expositivo?',
          imagen: require('@/assets/actividad/imagen5.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'El interpretativo solo enumera datos y excluye conclusiones.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'El interpretativo incorpora análisis, conclusiones y recomendaciones.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto:
                'El expositivo siempre busca obtener una aprobación formal.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'El interpretativo no puede incluir datos ni describir hechos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'El informe interpretativo no solo describe; también analiza la información y puede incluir conclusiones y recomendaciones.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
        {
          id: 20,
          texto:
            '¿Qué función cumplen los <em>dashboards</em> o tableros de visualización en inteligencia de negocios?',
          imagen: require('@/assets/actividad/imagen5.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Eliminar los datos de los sistemas de información.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Restringir la consulta de indicadores a documentos impresos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto: 'Reemplazar la necesidad de interpretar los resultados.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto:
                'Presentar datos mediante métricas, gráficos y tablas para apoyar la comprensión y la toma de decisiones.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Los dashboards visualizan información mediante indicadores, gráficos y tablas para facilitar su interpretación.',
          mensaje_incorrecto:
            'Revise nuevamente el contenido del componente formativo e intente responder la pregunta.',
        },
      ],
      mensaje_final_aprobado:
        '¡Excelente! Ha superado la actividad y demuestra una buena comprensión de los contenidos del componente formativo Recepción de requerimientos de clientes.',
      mensaje_final_reprobado:
        'Aún no ha superado la actividad. Le recomendamos revisar nuevamente el componente formativo e intentar otra vez la actividad didáctica.',
    },
  }),
}
</script>
