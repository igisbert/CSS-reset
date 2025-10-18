## Características

### Estructura base
- Aplica `box-sizing: border-box` a todos los elementos.   
- Elimina márgenes por defecto del `<body>` y establece una altura mínima con `min-height: 100lvh` para asegurar que cubra toda la pantalla, incluso con barras de dirección móviles.  
- Suaviza la tipografía en macOS y iOS con `-webkit-font-smoothing: antialiased`.  

### Propiedades modernas
- Usa `interpolate-size: allow-keywords` para permitir interpolaciones entre tamaños numéricos y keywords (`auto`, `fit-content`, etc.).  
- Añade `field-sizing: content` en `textarea` para ajustar automáticamente su tamaño al contenido.  

### Tipografía
- Utiliza `text-wrap: balance` en títulos (`h1–h6`) para equilibrar la longitud de las líneas y mejorar la legibilidad.  
- Aplica `text-wrap: pretty` en párrafos (`p`) para evitar saltos de línea incómodos y mejorar el flujo del texto.  
- Define `margin-block: 1lh` en párrafos, manteniendo una separación vertical proporcional al tamaño de línea.  

### Elementos multimedia
- Hace que `img`, `picture`, `svg`, `video` y `canvas` sean responsivos por defecto con `max-width: 100%` y `height: auto`.  

### Accesibilidad y usabilidad
- Añade soporte a `prefers-reduced-motion` reduciendo animaciones y transiciones cuando el usuario prefiere menos movimiento.  
- Desactiva el resalte azul en móviles con `-webkit-tap-highlight-color: transparent`.  
- Usa `scroll-behavior: smooth` para desplazamientos suaves, que se desactiva automáticamente si el usuario prefiere menos movimiento.  

### Enlaces y formularios
- Aplica `text-decoration-skip-ink: auto` para mejorar la legibilidad del subrayado en enlaces.  
- Evita el redimensionamiento manual de `textarea` (`resize: none`) para mantener la coherencia del diseño.  
