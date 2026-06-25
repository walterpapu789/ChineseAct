# Asian Wok - Página Principal (Landing Page) 🍜

**Integrantes:**  
Walter Steven López Espinoza  
Jefferson Adalberto Mejía Hernández  
Oscar Alexander Portillo Hernández

---

Este repositorio contiene el archivo `index.html` correspondiente a la página de inicio oficial de **Asian Wok**, una plataforma web de comida rápida especializada en platillos al wok con cobertura en El Salvador.

---

## 📋 Descripción del Documento

La página principal actúa como el eje central del sitio web. Está diseñada con un enfoque comercial y de experiencia de usuario, permitiendo explorar los productos estrella, conocer las categorías de comida disponibles y acceder rápidamente al sistema de pedidos.

### Características del Código:
* **Estructura Semántica de HTML5:** Organización limpia mediante `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` y `<footer>`.
* **Módulo de Autenticación:** Barra de acciones de usuario preparada para integrar flujos de inicio de sesión y visualización de carrito de compras.
* **Sección Hero Atractiva:** Presentación del gancho comercial ("Combo Red Dragon por $7.95") con llamadas a la acción (*Call to Action*).
* **Catálogo Organizado:** Grid de productos clasificados en dos grandes bloques: "Nuestras Comidas" y "Bebidas y Complementos".

---

## 🛠️ Arquitectura de la Página

El documento está estructurado de la siguiente manera de arriba a abajo:

### 1. Encabezado (`<header>`)
* **Logo Corporativo:** Ubicado en la esquina superior izquierda (`img/logo (2).png`).
* **Menú de Navegación:** Enlaces internos hacia `index.html`, `menu.html`, `promociones.html`, `nosotros.html` y `contacto.html`.
* **Área de Clientes (`.acciones-usuario`):** Acceso directo a `login.html` (icono de usuario) y un acceso para el carrito de compras.

### 2. Contenido Principal (`<main>`)
* **Sección Hero (`#inicio`):** Eslogan principal, descripción de oferta especial y botones interactivos (`Explorar Menú` y `Pedidos`).
* **Sección Catálogo (`#menu`):** Presentación estética de productos mediante tarjetas (`<article>`) organizadas en:
  * *Nuestras Comidas:* Combos, Arroces, Entradas y Banquetes.
  * *Bebidas y Complementos:* Bebidas, Promociones, Postres y Ofertas Dragón.

### 3. Pie de Página (`<footer>`)
* **Horarios de atención:** Desglose detallado por días de la semana.
* **Ubicaciones:** Listado de sucursales clave (San Salvador, Santa Tecla, Soyapango, Santa Ana, San Miguel).
* **Redes Sociales:** Enlaces externos con apertura en nueva pestaña (`target="_blank"`) para Facebook, Instagram y Twitter/X.
* **Créditos:** Nota de derechos reservados actualizada para el año 2026.

---

## 📂 Dependencias y Archivos Vinculados

Para que la página funcione con todo su potencial visual y lógico, se enlaza con los siguientes recursos:

* **Estilos CSS:** Localizados en `css/style.css`.
* **Scripts JS:** Carga el script de control de sesión en `../Proyecto/js/auth.js`.
* **Imágenes requeridas (`img/`):** 
  * Logo de marca: `logo (2).png`
  * Iconos: `inicioSesion.png`, `carritoCompras (2).png`
  * Recursos del menú: `cocina.png`, `combos.png`, `arroz.png`, `entradas.png`, `banquete.png`, `bebdias.png`, `promociones.png`, `postre.png`, `dragon.png`

---

## 💡 Notas para Desarrolladores

> 🛠️ **Integración de JavaScript:** Observa que en el `<head>` ya se encuentra vinculada la lógica de autenticación (`auth.js`). El contenedor `<div id="contenedor-autenticacion">` está preparado para que, mediante manipulación del DOM, cambie dinámicamente mostrando el nombre del usuario o un botón de "Cerrar Sesión" una vez que el cliente se haya autenticado.