# Living industrial · Sistema de diseño

Tipo de sitio: servicio. Muestra del kit de interiorismo de Nexvia IA para estudios.

Dirección editorial: fotografía del ambiente a sangre, lectura de izquierda a derecha y ritmo de lámina de presentación. La foto, el comparador, la maqueta, el plano y la lista explican decisiones distintas del mismo living.

## Sistema visual

| Token | Valor | Uso |
| --- | --- | --- |
| Marfil | `#F7F3EE` | Fondo principal y texto sobre grafito |
| Grafito | `#232120` | Texto, velo del hero y footer |
| Cuero | `#8A5A3B` | Acción principal, vista seleccionada, numeración editorial |
| Metal | `#1E1E1E` | Marcos, maqueta y acción oscura |
| Gris sofá | `#6E6E6E` | Texto secundario y materiales esquemáticos |
| Arena | `#EDE5DB` | Banda de la maqueta y del plano |
| Verde WhatsApp | `#25D366` | Acceso flotante con ícono blanco |

- Fraunces 400–500 para wordmark y títulos. Inter 400–600 para lectura, controles y precios.
- Escala de espacios de 4, 8, 12, 16, 24, 32, 48, 64, 96 y 128 px. Márgenes laterales parejos de 20 px a 430 px y hasta 72 px en escritorio. Ancho de lectura máximo de 1.280 px.
- Títulos de 48 a 112 px en el hero y de 34 a 64 px en secciones. Cuerpo de 16 px como base. Cifras tabulares en la lista.
- Botones rectangulares con esquinas de 5 px y foco visible. Fotos y láminas con esquinas de 8 px, sin sombras pesadas. El acceso flotante es de 58 px con sombra suave.
- Voz en español argentino. Los datos de la muestra se rotulan en el lugar donde se ven. Los controles de órbita y los enlaces al recorrido se distinguen por su nombre.

## Fotos elegidas

| Uso | Fuente | Archivo en el sitio |
| --- | --- | --- |
| Hero, después y frente | `media-generation-living-industrial-despues-0-354ddb3a-2d59-42ac-9dab-ecaf4eced28e.webp` adjunta | `assets/living-industrial-frente.webp` |
| Reversa | `Vista 2, desde los ventanales.webp` adjunta, equivalente de la toma pedida | `assets/living-industrial-reversa.webp` |
| Lateral | `media-generation-living-industrial-vista-latera-0-08cbe57d-7ca2-4afb-b0c5-287e7d455609.webp` adjunta. La otra toma lateral es idéntica byte a byte | `assets/living-industrial-lateral.webp` |
| Antes | Recreación generada a partir de la toma frontal. El archivo original no estaba en la ruta indicada ni en los archivos accesibles | `assets/living-vacio-recreacion.webp` |

La variante nórdica opcional se omite porque no se encontró el archivo. El comparador identifica el antes como recreación. Se generó con la herramienta de imágenes integrada, con la instrucción de retirar todos los muebles y objetos y preservar encuadre, arquitectura, ventanal, exterior e iluminación.

## Composición y comportamiento

1. Hero a pantalla completa. Encuadre industrial, velo desde el pie, aviso de muestra y dos acciones.
2. Comparador. Las imágenes comparten un encuadre. El deslizador admite arrastre, toque y teclado. Las etiquetas quedan legibles en los extremos.
3. Galería. La vista frontal abre la lámina. Reversa y lateral completan el mismo set, con los pies pedidos.
4. Maqueta. Modelo abierto esquemático, con Three.js y OrbitControls. Giro a demanda, tres cámaras y respaldo SVG cuando WebGL no está disponible.
5. Plano. Vista SVG con la misma orientación y piezas, leyenda y ninguna cota numérica.
6. Lista. Siete ítems y total en USD. Los valores son ejemplos ficticios y están identificados como tales.
7. Recorrido. Tarjeta enlazada al mundo de Marble indicado en el pedido. Abre en otra pestaña.
8. Kit. Cuatro entregables, la frase de 48 horas indicada en el pedido y contacto de Nexvia.
9. Footer grafito. Identidad de la muestra, aclaración y contacto.

El comparador y el cambio de cámara son los momentos interactivos. GSAP y ScrollTrigger animan brevemente la entrada del hero y el detalle gráfico del comparador. Lenis suaviza los saltos. Se respeta la preferencia de movimiento reducido y se mantiene el acceso por anclas y teclado.

Todos los botones de WhatsApp referencian el mismo símbolo SVG provisto. Los botones y enlaces no hacen envíos automáticos.
