# practica-unidad4
# PARTE 1: Investigación y Preparación

## 1. Diferencia técnica: ¿Cómo cambia la lógica del servidor al consumir una API de base de datos vs. una API de IA (como Gemini)?
Una API de base de datos está diseñada para almacenar, consultar y manipular información estructurada. El servidor realiza operaciones como insertar registros, actualizar datos o consultar información específica utilizando comandos definidos.

Ejemplo:
- Guardar usuarios
- Consultar productos
- Actualizar información

En cambio, una API de Inteligencia Artificial trabaja con modelos capaces de interpretar lenguaje natural, generar contenido y responder dinámicamente a instrucciones llamadas prompts.

Ejemplo:
- Generar texto
- Responder preguntas
- Crear imágenes
- Resumir información

### Diferencia en la lógica del servidor

Cuando el servidor consume una API de base de datos:
- Se realizan operaciones CRUD.
- Las respuestas son exactas y estructuradas.
- El flujo es predecible.

Cuando el servidor consume una API de IA:
- El servidor construye prompts.
- Se valida y sanitiza texto antes de enviarlo.
- Las respuestas pueden variar.
- Se requiere manejo adicional de contexto y tokens.

---

## 2. Seguridad: ¿Por qué es una vulnerabilidad grave exponer una API Key en el frontend y cómo ayuda el backend a protegerla?

Una API Key es una credencial privada que permite acceder a servicios externos como Gemini API.

Si la API Key se coloca en el frontend:
- Cualquier usuario puede verla usando las herramientas del navegador.
- La clave puede ser robada y utilizada por terceros.
- Se pueden generar cargos no autorizados.
- Existe riesgo de abuso del servicio.

### ¿Cómo ayuda el backend?

El backend protege la API Key porque:
- La clave permanece oculta en el servidor.
- El navegador nunca tiene acceso directo.
- El servidor actúa como intermediario seguro.
- Se pueden aplicar validaciones y restricciones.

### Flujo seguro

Usuario → Frontend → Backend → Gemini API

De esta forma, la clave nunca se expone públicamente.

---

## 3. Herramientas: ¿Qué es Google AI Studio y para qué sirve en el flujo de desarrollo?

Google AI Studio es una plataforma de Google diseñada para probar y desarrollar aplicaciones basadas en modelos Gemini.

Permite:
- Probar prompts.
- Experimentar con modelos de IA.
- Ajustar parámetros.
- Generar código de integración.
- Crear prototipos rápidos.

### Importancia en el desarrollo

Google AI Studio facilita el proceso de desarrollo porque:
- Permite probar ideas antes de programar.
- Ayuda a optimizar prompts.
- Reduce errores de integración.
- Genera ejemplos en distintos lenguajes.

### Flujo de trabajo típico

1. Diseñar prompt en Google AI Studio.
2. Probar respuestas.
3. Ajustar parámetros.
4. Generar código.
5. Integrar en backend Node.js o PHP.
