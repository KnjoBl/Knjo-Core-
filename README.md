KNJO-IA

Asistente personal de inteligencia artificial para Android.

KNJO-IA es un proyecto independiente de KNJO Systems™ orientado a construir un asistente conversacional instalable en Android, con interacción por texto, voz y memoria personal controlada por el usuario.

Estado del proyecto

Fase actual: Arquitectura definida; implementación pendiente.

Este repositorio inicia el desarrollo de KNJO-IA. Las funciones descritas a continuación son objetivos de diseño, no capacidades ya implementadas o verificadas.

Objetivos

- Aplicación Android nativa: Kotlin y Jetpack Compose.
- Conversación por texto: interfaz de chat.
- Inteligencia artificial: integración inicial prevista con Google Gemini mediante un backend seguro.
- Interacción por voz: entrada por voz y respuestas habladas.
- Conversación continua por voz: modo opcional, visible y controlado por el usuario.
- Memoria controlada: guardar información únicamente con autorización explícita, con opciones para consultar, editar y eliminar los datos guardados.
- Privacidad y seguridad: no incluir claves privadas de proveedores de IA dentro de la aplicación Android.
- Arquitectura ampliable: permitir incorporar otros proveedores en el futuro.

Primera versión prevista

La primera entrega será una aplicación Android con una conversación simulada localmente, identificada claramente como SIMULADO.

Esta versión inicial no realizará llamadas a servicios de IA, no requerirá conexión a Internet y no implementará todavía voz ni memoria persistente.

Arquitectura prevista

- "android/" — aplicación Android.
- "backend/" — servicio intermediario para proveedores de IA, en una fase posterior.
- "docs/" — especificaciones, decisiones y documentación técnica.
- "contracts/" — contratos de API cuando se implemente el backend.
- "tests/" — pruebas automatizadas.

La estructura anterior es propuesta y podrá ajustarse durante la implementación, documentando los cambios.

Principios de desarrollo

1. Evidencia antes que suposiciones.
2. Verificación antes que declaraciones de éxito.
3. Conservar intactos los archivos originales de referencia.
4. Separar claramente lo diseñado, implementado, probado y validado.
5. Proteger las credenciales y los datos personales.
6. No desplegar servicios ni generar costes sin autorización explícita.
7. No modificar proyectos externos ni recursos de KNJO Systems™ sin autorización.

Alcance y separación

KNJO-IA será un proyecto independiente. El prototipo KNJO-M podrá utilizarse como referencia visual cuando corresponda, pero no se considerará una base técnica Android ni se modificará su archivo original.

Este proyecto tampoco autoriza cambios en KNJO Core, Netlify o servicios de Cloudflare.

Licencia

Sin licencia asignada por el momento. El código no debe considerarse de uso libre hasta que se establezca una licencia explícita.

Nota de estado

La existencia de este documento no significa que la aplicación, el backend, la integración con Gemini, la memoria o la voz estén implementados. Cada función se marcará como implementada, probada o validada únicamente cuando exista evidencia verificable.
