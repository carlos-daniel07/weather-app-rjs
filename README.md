# 🌦️ Aplicación del Clima - Integración de API REST y Material UI

Aplicación web desarrollada en React para la consulta meteorológica en tiempo real mediante la integración de servicios de terceros (WeatherAPI). El proyecto destaca por la implementación de una interfaz visual construida con Material UI (MUI), gestión de feedback visual asíncrono y control de variables de entorno seguras.

🔗 **[Ver Demo en Vivo](https://weather-app-react-js-course.netlify.app/)**

## 🚀 Arquitectura y Características

* **Consumo de API Externa:** Peticiones asíncronas optimizadas utilizando la API Fetch (`async/await`) contra los endpoints de WeatherAPI.
* **Componentes de Interfaz Empresarial:** Implementación del ecosistema `@mui/material` y `@mui/lab` (`Container`, `TextField`, `LoadingButton`, `Typography`) para un diseño limpio y accesible.
* **Gestión de Carga y Feedback Visual:** Uso del componente `LoadingButton` para deshabilitar interacciones durante la resolución de promesas y evitar peticiones duplicadas.
* **Manejo Integral de Excepciones:** Control estructurado de errores con bloques `try/catch/finally`, validando campos vacíos y errores HTTP directos de la API.
* **Seguridad y Entorno:** Manejo desacoplado de credenciales y endpoints mediante variables de entorno en Vite (`import.meta.env.VITE_API_KEY`).

## 🛠️ Tecnologías Utilizadas

* **React (ES6+)**
* **Material UI (MUI v5)**
* **Notistack** (Sistema de notificaciones)
* **WeatherAPI** (REST API)
* **Vite**

## 🧠 Retos Técnicos
El principal desafío consistió en sincronizar de forma reactiva las respuestas de la API con los estados visuales de la aplicación. Se implementó una estructura de estados modular para segregar los datos del clima (`weather`), el estado de red (`loading`) y las alertas de validación (`error`), garantizando una experiencia de usuario fluida incluso ante fallos de conexión o entradas erróneas.
