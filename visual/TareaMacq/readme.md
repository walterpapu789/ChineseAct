## Documentación Técnica

### ¿Por qué utilizamos Grid para separar el panel lateral del contenido principal en lugar de Flexbox?

Utilizamos CSS Grid para la estructura macro porque está diseñado para controlar el diseño en dos dimensiones (filas y columnas) al mismo tiempo, permitiendo definir un mapa rígido y predecible (`grid-template-areas`) para el esqueleto del sitio. Intentar maquetar la estructura global únicamente con Flexbox obligaría a forzar una herramienta unidimensional (hecha para un solo eje) a comportarse de forma bidimensional, complicando el código y perdiendo el control simétrico sobre la alineación simultánea de la barra superior, el menú lateral y la sección de contenido.