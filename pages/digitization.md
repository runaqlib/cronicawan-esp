---
layout: page
title: Sobre el proyecto de digitalización 
permalink: /digitization-project/
---


<a href="{{ '/img/cbc.png' | absolute_url }}">
  <img src="{{ '/img/cbc.png' | absolute_url }}" alt="Una vista del exterior del Centro Bartolomé de las Casas en Cusco, Perú."/>
</a>

_Alt: Una vista del exterior del Centro Bartolomé de las Casas en Cusco, Perú._

### Encontrar los periódicos

Los fondos de la subvención Tinker me permitieron viajar al Centro Bartolomé de las Casas (CBC) en Cusco y comenzar el proceso de digitalización, transcripción y traducción de estos trabajos para trabajar en mi tesis para Estudios Latinoamericanos y Caribeños en NYU. Las 15 ediciones disponibles en el archivo habían estado claramente expuestas al agua y otros elementos, que estaban empezando a degradar el papel y a hacer que los periódicos fueran frágiles. Los números se digitalizaron utilizando una configuración con un trípode modificado, mi iPhone y la aplicación Adobe Scan.

<img src="{{ '/img/setup.png' | absolute_url }}" alt="A photo of the digitization setup, including a table, copies of the newspapers, a tripod, and a laptop showing scans of the issues."/>

_Alt: Una foto de la configuración de la digitalización, que incluye una mesa, copias de los periódicos, un trípode y una computadora que muestra escaneos de los números._

### Transcripciones: a mano, la automatización y los límites de la tecnología

_Cronicawan_ fue publicado casi en su totalidad en quechua, un idioma que sigue siendo en gran parte oral y ha sido marginado durante mucho tiempo. Las herramientas tradicionales OCR (reconocimiento óptico de caracteres), normalmente entrenadas en impresión latina en inglés o español, no fueron capaces de leer con precisión el idioma quechua o interpretar los diseños de página del periódico.

Utilicé [Transkribus](https://www.transkribus.org/), una plataforma que utiliza modelos de lenguaje de IA para el reconocimiento automatizado de texto, para entrenar un modelo de IA personalizado específicamente diseñado para reconocer el texto de Cronicawan. Esto permitió un mayor grado de precisión que otras herramientas de OCR preexistentes. Incluso con esta herramienta, el proceso de transcripción requirió intervención humana.

**Las transcripciones disponibles en este sitio son una combinación de texto transcrito a mano, corregido a mano y automatizado** especialmente cuando el daño de página, el texto estilizado o el espaciado inusual hacen que los resultados no sean confiables. Dicho esto, **Las transcripciones automatizadas pueden no ser 100% precisas, así que por favor tenga cuidado y revise el texto.** Por favor, póngase en contacto conmigo si nota errores de transcripción mientras navega.

<img src="{{ '/img/transkribus.gif' | absolute_url }}" alt="A gif of the Transkribus UI, showing the process of hand-correcting AI-detected text."/>

*Alt: Un gif de la interfaz de usuario de Transkribus, que muestra el proceso de corrección manual del texto detectado por IA.*

### Traducciones e interpretaciones
Translation presentó su propio conjunto de desafíos con Cronicawan. He tomado la **decisión deliberada de no traducir el texto quechua al inglés o al español más allá de las traducciones al español que se incluyeron en el propio periódico**. Esta decisión refleja tanto la complejidad cultural de la traducción del quechua como las limitaciones de las herramientas de traducción automatizada o no experta a la hora de manejar matices lingüísticos.

**Las traducciones al inglés están automatizadas a partir de las traducciones al español proporcionadas, así que ten cuidado al navegar.** Se invita a los visitantes a interactuar con los textos en quechua tal como están, sin editar, con su contexto histórico y riqueza lingüística intacta.

---

### Construyendo el sitio web: Jekyll, Wax y una vista en el archivo

Este proyecto está impulsado por el compromiso de hacer que los materiales en quechua sean más accesibles y visibles en línea, al tiempo que es consciente de las limitaciones tecnológicas y culturales inherentes al trabajo con lenguajes y formatos de archivo subrepresentados. Esta edición de Cronicawan, **publicada 50 años después de su publicación inicial, ofrece una nueva forma de conocer y estudiar este raro periódico en lengua quechua**.

_La digitalización de Cronicawan_ se construyó utilizando Jekyll, un generador de sitios estáticos. Utilicé Wax, un framework para Jekyll diseñado para soportar colecciones basadas en imágenes. Wax me permitió formatear más fácilmente páginas individuales para cada edición y transcripción con sus metadatos asociados, e implementar funciones de búsqueda en todos los documentos. El visor de transcripciones permite a los usuarios ver transcripciones en quechua y español junto con imágenes escaneadas del periódico original.