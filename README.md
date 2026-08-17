# cssrespaldo
Solo es respaldo css de pagina web wander 
@import url('https://fonts.googleapis.com/css2?family=Carter+One&display=swap');


/* ==========================================================================
   1. REGLAS GLOBALES Y ESCUDOS ESTRUCTURALES
   ========================================================================== */
html, body {
    overflow-x: hidden !important;
    width: 100% !important;
    max-width: 100vw !important;
    position: relative;
}

/* Solución del Footer pegado al fondo (Flexbox) */
body, .wp-site-blocks {
    display: flex !important;
    flex-direction: column !important;
    min-height: 100vh !important;
    margin: 0;
}

.wp-site-blocks {
    flex: 1 0 auto !important;
    width: 100%;
}

footer, .wp-block-template-part-footer {
    margin-top: auto !important;
    width: 100%;
}

/* ==========================================================================
   2. FIX DEFINITIVO: CABECERA Y TEXTO CENTRADO (El bloque que desaparecía)
   ========================================================================== */
header, 
.wp-block-template-part-header, 
header .wp-block-group {
    overflow: visible !important;
    overflow-x: visible !important;
    overflow-y: visible !important;
}

.hidden-default,
.wp-block-items-justified-center > .wp-block-group {
    display: flex !important; 
    opacity: 1 !important;
    visibility: visible !important;
    pointer-events: auto !important;
    
    /* Centrado Matemático Absoluto */
    position: absolute !important;
    top: 75px !important; /* Ajusta este valor si choca con tu menú */
    left: 50% !important;
    transform: translateX(-50%) !important;
    
    z-index: 9999999 !important; 
    width: 90% !important;
    max-width: 350px !important;
    justify-content: center !important;
}

/* ==========================================================================
   3. TIPOGRAFÍA, ENLACES Y CONTENIDO PRINCIPAL
   ========================================================================== */
/* Estado normal y hover del enlace */
.entry-content a {
    text-decoration: none !important;
    color: #008000 !important;
    transition: all 0.2s ease-in-out !important;
}

.entry-content a:hover,
.entry-content a:focus {
    color: #00da00 !important; 
    text-decoration: underline !important;
}

/* Forzar fuente y tamaño en Encabezados */
.main_content h1 {
    font-family: 'Carter One', display, sans-serif !important;
    font-size: 28px !important;
    font-weight: normal !important;
    line-height: 1.2 !important;
}

.main_content h2 {
    font-family: 'Carter One', display, sans-serif !important;
    font-size: 25px !important;
    line-height: 1.0 !important;
    padding-top: 0 !important;
    padding-bottom: 0 !important;
}

.entry-content h3 {
    font-family: 'Carter One', display, sans-serif !important;
    font-size: 20px !important;
    font-weight: normal !important;
    line-height: 1.4 !important;
}

/* Contenedor principal y espaciado de Párrafos */
.main_content {
    width: 100%; 
}

.main_content p {
    margin-top: 0 !important;
    margin-bottom: 12px !important;
    padding-top: 0 !important;
    padding-bottom: 0 !important;
    line-height: 1.3 !important;
    display: block !important; 
    min-height: 1.5em !important;
}

.main_content p:empty {
    min-height: 0.5em !important;
    margin-bottom: 3px !important;
}

/* Imágenes y Adjuntos */
.attachment-medium {
    width: 310px !important;
    height: 440px !important;
    display: block !important;
    object-fit: cover !important;
    vertical-align: top !important;
    box-sizing: border-box !important;
    padding: 1px 2px 2px 1px !important;
    padding-bottom: 13px; 
    background-color: #000000 !important; 
    border: none !important;
    outline: none !important;
    box-shadow: none !important;
    pointer-events: none !important;
}

.photo_campana {
    display: flex; 
    width: 100% !important;
    max-width: auto !important;
    margin: 0 auto !important;
    display: block !important;
    text-align: center !important;
}

.photo_campana img {
    width: auto !important;
    height: auto !important;
    border: solid 2px black !important;
    border-radius: 3px !important;
    display: inline-block !important;
}

/* Info ficha técnica y columnas */
.info_ficha {
    margin-left: 10px;
    margin-top: 5%; 
    width: 80%;
}

.Ficha_photo { 
    height: 130%;
    margin-right: 3%;
    width: 50%;
}

.Ficha_column {
    border: 1px solid #f0f0f0; 
    background: #fff;
    height: 110%;
    margin-right: 3%;
    width: 50%;
}

.Ficha_column p {
    margin-top: 0 !important;
    margin-bottom: 12px !important;
    padding-top: 0 !important;
    padding-bottom: 0 !important;
    line-height: 1.3 !important;
    display: block !important; 
    min-height: 1.5em !important;
}

.Ficha_column p:empty {
    min-height: 0.5em !important;
    margin-bottom: 3px !important;
}

.Ficha_column a {
    color: #008000 !important;
    transition: color 0.2s ease-in-out !important; 
}

.wp-block-column.Ficha_column {
    margin-top: 0 !important;
}

.column_center {
    align-content: center; 
    justify-content: center; 
    margin-right: 9%; 
}

.tittles {
    color: #006B39; 
    font-style: italic; 
    font-size: 1.5em;
}

/* Ocultar elementos específicos y utilidades */
body > div.wp-site-blocks > div.wp-block-columns.is-layout-flex.wp-container-core-columns-is-layout-28f84493.wp-block-columns-is-layout-flex > div.wp-block-column.Ficha_column.has-border-color.is-layout-flow.wp-container-core-column-is-layout-4b4fa397.wp-block-column-is-layout-flow > div > div > div.pods-all-fields-row.pods-all-fields-row-name-titulos-y-logros > strong {
    display: none;
}

body > div.wp-site-blocks > div.wp-block-columns.is-layout-flex.wp-container-core-columns-is-layout-28f84493.wp-block-columns-is-layout-flex > div.wp-block-column.Ficha_column.has-border-color.is-layout-flow.wp-container-core-column-is-layout-4b4fa397.wp-block-column-is-layout-flow > div > div > div.pods-all-fields-row.pods-all-fields-row-name-instagram {
    display: flex; 
}

body > div.wp-site-blocks > div.wp-block-columns.is-layout-flex.wp-container-core-columns-is-layout-bb6ee2e1.wp-block-columns-is-layout-flex > div.wp-block-column.Ficha_column.has-border-color.is-layout-flow.wp-container-core-column-is-layout-4b4fa397.wp-block-column-is-layout-flow > div > div > div.pods-all-fields-row.pods-all-fields-row-name-titulos-y-logros > strong {
    display: none;
}

.column_photo_player {
    justify-content: flex-start;
    margin-top: 30px;
    height: 100%; 
}

.migajas {
    color: white;
}

.migajas a {
    color: white;
    margin-left: 10%;
}

.fuente_img {
    margin-left: 10%;
}

.pods-all-fields-row-name-instagram {
    display: flex; 
}

.hover-verde-wanderers a:hover {
    text-decoration: underline !important;
    text-decoration-color: #00FF00 !important;
}

.input_search {
    width: 20%; 
}

.name_player {
    color: white;
    font-family: "Carter One" !important; 
    line-height: 1.2 !important;
    margin-bottom: 0 !important; 
    margin-top: 0 !important;
}

/* Banner Jugadores y Vistas */
.wp-block-kadence-column .name_player p {
    font-family: "Carter One" !important;
    font-size: 1.9rem !important; 
    max-width: 70%;
    transform: translateX(0px) translateY(0px);
    position: relative;
    left: 39%;
    top: 21px;
    padding-left: 0px !important;
    margin-left: 34% !important;
    margin-top: 1% !important;
    font-weight: 400; 
    color: #ffffff !important;
}

body .wp-site-blocks .wp-block-kadence-column .name_player p {
    color: #ffffff !important; 
    font-family: "Carter One" !important;
    margin-left: 20px !important;
    margin-right: 0 !important;
    padding: 0 !important;
    font-size: 2rem !important;
}

.post-views {
    font-size: 0.9rem;
    color: #666;
    background: #f5f5f5;
    padding: 5px 10px;
    border-radius: 20px;
    display: inline-flex;
    align-items: center;
}

.post-views-icon.dashicons::before {
    content: "⚽" !important; 
    font-family: Arial, sans-serif !important; 
    font-size: 1.1em; 
    margin-right: 3px;
    vertical-align: middle;
}

/* Forzar Columna Vertical en el bloque partidos */
#guten-fbuXK3,
#guten-fbuXK3 > .stk-row, 
#guten-fbuXK3 > .stk-content-inner {
    display: flex !important;
    flex-direction: column !important; 
    flex-wrap: wrap !important;
}

#guten-fbuXK3 > *,
#guten-fbuXK3 .stk-column {
    width: 100% !important;
    max-width: 100% !important;
    flex-basis: 100% !important; 
    margin-left: 0 !important;
    margin-right: 0 !important;
}

.wp-block-kadence-column .yoast-breadcrumbs {
    font-size: 12px;
    text-align: center; 
    color: white;
    font-family: "Carter one";
    margin-top: -10px !important; 
    padding-top: 0 !important;
    position: relative; 
    z-index: 10;
}

.wp-block-kadence-column .yoast-breadcrumbs a {
    color: #808080 !important; 
}

.wp-block-kadence-column .yoast-breadcrumbs a:hover {
    color: #505050 !important;
}

/* Forzar fuentes en enlaces */
body .wp-site-blocks .Ficha_column a,
body .wp-block-pods-pods-block-field a,
body .wp-block-kadence-column .kt-inside-inner-col a,
body .wp-block-kadence-column .kt-inside-inner-col p a {
    text-decoration: none !important; 
    color: #008000 !important;
    transition: all 0.2s ease-in-out !important; 
}

body .wp-site-blocks .Ficha_column a:hover,
body .wp-site-blocks .Ficha_column a:focus,
body .wp-block-pods-pods-block-field a:hover,
body .wp-block-pods-pods-block-field a:focus,
body .wp-block-kadence-column .kt-inside-inner-col a:hover,
body .wp-block-kadence-column .kt-inside-inner-col a:focus,
body .wp-block-kadence-column .kt-inside-inner-col p a:hover,
body .wp-block-kadence-column .kt-inside-inner-col p a:focus {
    color: #00da00 !important; 
    text-decoration: underline !important;
}

/* Diseño de columna de lectura */
.contenido-campana {
    display: block !important;
    width: 100% !important;
}

.contenido-campana p {
    text-align: left !important; 
    width: 59% !important; 
    margin-left: auto !important; 
    margin-right: auto !important;
}

.contenido-campana h1,
.contenido-campana h2,
.contenido-campana h3,
.contenido-campana h4 {
    text-align: center !important;
    width: 75% !important;
    margin-left: auto !important;
    margin-right: auto !important;
}

.contenido-campana img,
.contenido-campana .aligncenter,
.contenido-campana figure.wp-caption {
    display: block !important;
    margin-left: auto !important;
    margin-right: auto !important;
}

.contenido-campana .wp-caption-text {
    text-align: center !important;
    width: 100% !important;
}

/* Template nuevo páginas (Columnas) */
.caja-blanca-contenido ul {
    column-count: 3; 
    column-gap: 40px; 
    list-style-type: none; 
    padding-left: 0;
}

.caja-blanca-contenido ul li {
    break-inside: avoid;
    page-break-inside: avoid;
    margin-bottom: 12px;
    font-size: 15px;
    line-height: 1.5;
}

/* Forzar tipografía en Pods */
.wp-block-pods-pods-block-field p,
.wp-block-pods-pods-block-field span,
.wp-block-pods-pods-block-field div,
.wp-block-pods-pods-block-field li {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen-Sans, Ubuntu, Cantarell, "Helvetica Neue", sans-serif !important;
    font-size: 15px !important;
}


/* ==========================================================================
   4. MEDIA QUERIES (RESPONSIVE)
   ========================================================================== */

/* 4.1 MÓVIL: Todo lo que mida 768px o menos (Smartphones) */
@media (max-width: 768px) {
    
    /* =========================================================
       1. REGLAS ESTRUCTURALES MÓVILES
       ========================================================= */
    .wp-site-blocks {
        display: flex;
        flex-direction: column;
        min-height: 100vh; 
    }

    main {
        flex-grow: 1;
    }
    
    .caja-blanca-contenido ul {
        column-count: 2; 
    }
    
    main.wp-block-group, 
    .wp-block-post-content {
        display: block !important;
        width: 100% !important;
        min-height: 50vh !important;
        padding-left: 15px !important;
        padding-right: 15px !important;
    }
    
    .name_player_mobile,
    .name_player_mobile * {
        color: #ffffff !important; 
        font-family: 'Carter One' !important;
        font-size: 1rem;
        line-height: 1.2 !important; 
        display: flex; 
        text-align: center;
        align-content: center; 
        align-items: center; 
        height: auto !important;
        max-width: 100% !important;
    }   
    
    .Ficha_column2 {
        border: 1px solid #f0f0f0; 
        background: #fff;
        height: 100%;
        width: 50%;
    }

    /* =========================================================
       2. CENTRADO DEFINITIVO DE IMÁGENES Y LEYENDAS (CAMPAÑAS)
       ========================================================= */

    /* Contenedor principal de la imagen */
    .contenido-campana figure.wp-caption,
    .contenido-campana .wp-block-image,
    .contenido-campana .alignnone {
        display: block !important;
        width: 100% !important;
        margin: 0 auto !important;
        float: none !important;
        text-align: center !important; 
			
    }

    /* La imagen física (Anulamos el right: 30vw destructivo) */
    .contenido-campana figure.wp-caption img,
    .contenido-campana .wp-block-image img,
    .contenido-campana .alignnone img,
    .wp-site-blocks .wp-caption img {
        display: inline-block !important; 
        margin: 0 auto !important;
        max-width: 100% !important;
        width: 100% !important; /* Obliga a llenar el espacio disponible en móvil */
        height: auto !important;
        position: static !important; /* Anula posiciones forzadas */
        right: auto !important; 
        left: auto !important;
    }

    /* Reset absoluto de la leyenda y sus párrafos internos */
    .contenido-campana figure figcaption,
    .contenido-campana figure .wp-caption-text,
    .contenido-campana figure .wp-element-caption,
    .contenido-campana figure figcaption p,
    .contenido-campana figure .wp-caption-text p,
    .contenido-campana figure .wp-element-caption p {
        position: static !important;
        transform: none !important;
        display: block !important;
        
        width: 100% !important; /* Mata la regla del 59% y del 130vw */
        max-width: 100% !important;
        
        margin: 15px 0 10px 0 !important; 
        padding: 0 10px 15px !important; 
        
        text-align: center !important; 
        box-sizing: border-box !important;
        left: 0 !important;
        right: 0 !important;
    }

    /* =========================================================
       3. ADAPTACIÓN MÓVIL PARA EL MENÚ/TÍTULO
       ========================================================= */
    .wp-block-navigation__responsive-container.is-menu-open {
        position: fixed !important;
        top: 50% !important; 
        left: 50% !important;
        transform: translate(-50%, -60%) !important; 
        width: 85vw !important; 
        max-width: 400px !important; 
        height: auto !important; 
        min-height: 250px !important; 
        max-height: 85dvh !important; 
        overflow-y: auto !important; 
        margin: 0 !important;
        right: auto !important;
        bottom: auto !important;
        background-color: #ffffff !important;
        box-shadow: 0 15px 40px rgba(0, 0, 0, 0.4) !important; 
        border-radius: 12px !important; 
        z-index: 99999 !important;
    }

    html.has-modal-open,
    body.has-modal-open {
        overflow: auto !important;
    }
    
    .wp-block-navigation__responsive-container-close {
        display: flex !important;
        position: absolute !important;
        top: 15px !important; 
        right: 20px !important; 
        color: #000000 !important; 
        background: transparent !important;
        border: none !important;
        z-index: 100000 !important; 
    }
    
    .wp-block-navigation__responsive-container-content {
        padding: 20px 20px 20px 40px !important; 
        align-items: flex-start !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-navigation-item a {
        color: #00703c !important; 
        font-weight: bold !important;
        text-transform: uppercase !important;
        padding-bottom: 12px !important; 
        font-size: 13px !important; 
    }

    .wp-block-navigation__responsive-container-open {
        position: absolute !important; 
        top: 50% !important; 
        transform: translateY(-50%) !important; 
        color: #00703c !important; 
        background: transparent !important;
        border: none !important;
        padding: 0 !important;
        z-index: 9999 !important; 
    }

    .wp-block-navigation__responsive-container-open svg {
        fill: #00703c !important; 
        width: 35px !important; 
        height: 35px !important;
    }

    .wp-block-navigation__responsive-container-content .wp-block-search {
        margin-top: 10px !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-search__input {
        padding: 8px 12px !important; 
        font-size: 14px !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-search__button {
        padding: 8px 15px !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-navigation-item a,
    .wp-block-navigation__responsive-container-content .wp-block-search__input,
    .wp-block-navigation__responsive-container-content .wp-block-search__button {
        font-family: 'Carter One', cursive !important;
        font-weight: normal !important; 
    }
}
/* 4.2 TABLET: Entre 769px y 1024px (Pads y Laptops pequeñas) */
@media (min-width: 769px) and (max-width: 1024px) {
    
    /* =========================================================
       1. CONTENEDOR PRINCIPAL
       ========================================================= */
    main.wp-block-group, 
    .wp-block-post-content {
        display: block !important;
        width: 90% !important; 
        max-width: 850px !important; 
        margin: 0 auto !important; 
        padding-left: 30px !important; 
        padding-right: 30px !important;
    }
    
    .kadence-column1322_126e6c-f9 > div:nth-child(1) {
        margin-left: 5%;
    }

    /* =========================================================
       2. CENTRADO DEFINITIVO DE IMÁGENES Y LEYENDAS (LIMPIO)
       ========================================================= */
    .contenido-campana figure.wp-caption,
    .contenido-campana .wp-block-image,
    .contenido-campana .alignnone {
        display: block !important;
        width: 100% !important;
        margin: 0 auto !important;
        float: none !important;
        text-align: center !important; 
    }

    /* Imagen física (Anula los desplazamientos en vw) */
    .contenido-campana figure.wp-caption img,
    .contenido-campana .wp-block-image img,
    .contenido-campana .alignnone img,
    .wp-site-blocks .wp-caption img,
    .wp-site-blocks .wp-block-group .wp-block-group .wp-block-pods-pods-block-field .wp-caption img {
        display: inline-block !important; 
        margin: 0 auto !important;
        max-width: 100% !important;
        width: 100% !important;
        height: auto !important;
        position: static !important; 
        right: auto !important; 
        left: auto !important;
    }

    /* Leyenda (Caption) y párrafos internos */
    .contenido-campana figure figcaption,
    .contenido-campana figure .wp-caption-text,
    .contenido-campana figure .wp-element-caption,
    .contenido-campana figure figcaption p,
    .contenido-campana figure .wp-caption-text p,
    .contenido-campana figure .wp-element-caption p,
    .wp-site-blocks .wp-block-group .wp-block-group .wp-block-pods-pods-block-field .wp-caption .wp-caption-text,
    .wp-site-blocks .wp-block-group .wp-caption {
        position: static !important;
        transform: none !important;
        display: block !important;
        
        width: 100% !important; /* Mata la compresión del 55% y el desbordamiento de 130vw */
        max-width: 100% !important;
        
        margin: 15px 0 0 0 !important; 
        padding: 0 20px !important; /* Un poco más de respiro lateral para tablets */
        
        text-align: center !important; 
        box-sizing: border-box !important;
        left: 0 !important;
        right: 0 !important;
    }

    /* =========================================================
       3. ADAPTACIÓN MENÚ HAMBURGUESA TABLET
       ========================================================= */
    .wp-block-navigation__responsive-container.is-menu-open {
        position: fixed !important;
        top: 50% !important; 
        left: 50% !important;
        transform: translate(-50%, -60%) !important; 
        width: 85vw !important; 
        max-width: 400px !important; 
        height: auto !important; 
        min-height: 250px !important; 
        max-height: 85dvh !important; 
        overflow-y: auto !important; 
        margin: 0 !important;
        right: auto !important;
        bottom: auto !important;
        background-color: #ffffff !important;
        box-shadow: 0 15px 40px rgba(0, 0, 0, 0.4) !important; 
        border-radius: 12px !important; 
        z-index: 99999 !important;
    }

    html.has-modal-open,
    body.has-modal-open {
        overflow: auto !important;
    }
    
    .wp-block-navigation__responsive-container-close {
        display: flex !important;
        position: absolute !important;
        top: 15px !important; 
        right: 20px !important; 
        color: #000000 !important; 
        background: transparent !important;
        border: none !important;
        z-index: 100000 !important; 
    }
    
    .wp-block-navigation__responsive-container-content {
        padding: 20px 20px 20px 40px !important; 
        align-items: flex-start !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-navigation-item a {
        color: #00703c !important; 
        font-weight: bold !important;
        text-transform: uppercase !important;
        padding-bottom: 12px !important; 
        font-size: 13px !important; 
    }

    .wp-block-navigation__responsive-container-open {
        position: absolute !important; 
        top: 50% !important; 
        transform: translateY(-50%) !important; 
        color: #00703c !important; 
        background: transparent !important;
        border: none !important;
        padding: 0 !important;
        z-index: 9999 !important; 
    }

    .wp-block-navigation__responsive-container-open svg {
        fill: #00703c !important; 
        width: 35px !important; 
        height: 35px !important;
    }

    .wp-block-navigation__responsive-container-content .wp-block-search {
        margin-top: 10px !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-search__input {
        padding: 8px 12px !important; 
        font-size: 14px !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-search__button {
        padding: 8px 15px !important; 
    }

    .wp-block-navigation__responsive-container-content .wp-block-navigation-item a,
    .wp-block-navigation__responsive-container-content .wp-block-search__input,
    .wp-block-navigation__responsive-container-content .wp-block-search__button {
        font-family: 'Carter One', cursive !important;
        font-weight: normal !important; 
    }
}

/* 4.3 ESCRITORIO: Todo lo que mida 1025px o más (Monitores) */
@media (min-width: 1025px) {
    
    ul.wp-block-navigation__container {
        display: flex !important;
        flex-direction: row !important;
        width: 100% !important; 
        justify-content: space-between !important;
        gap: 0 !important; 
        padding: 0 !important;
    }

    ul.wp-block-navigation__container > .wp-block-navigation-item {
        flex-grow: 1 !important; 
        display: flex !important;
        justify-content: center !important; 
        align-items: center !important;
    }
}

@media (max-width: 1024px) {
    
    /* ==========================================================================
       1. REPARACIÓN DEL BANNER DE TÍTULOS
       ========================================================================== */
    
    /* Ajuste del contenedor principal (Fondo de lluvia/estadio) */
    .wp-block-group.block-visibility-hide-large-screen {
        display: flex !important;
        align-items: center !important;
        justify-content: center !important;
        min-height: 180px !important; /* Altura segura para que no se aplaste */
        height: auto !important;
        padding: 20px 15px !important; /* Respiro lateral */
    }

    /* Ajuste de la caja verde interior (Overlay) */
    .wp-block-group.block-visibility-hide-large-screen > .wp-block-group {
        width: 95% !important;
        max-width: 700px !important;
        margin: 0 auto !important;
        padding: 20px !important; /* Infla la caja para que el texto no toque los bordes */
        height: auto !important;
        display: flex !important;
        flex-direction: column !important;
        justify-content: center !important;
    }

    /* Domar el texto del título para que salte de línea ordenado */
    .wp-block-group.block-visibility-hide-large-screen h1,
    .wp-block-group.block-visibility-hide-large-screen h2,
    .wp-block-group.block-visibility-hide-large-screen h3,
    .wp-block-group.block-visibility-hide-large-screen p {
        text-align: center !important;
        font-size: 24px !important; /* Tamaño legible y proporcional */
        line-height: 1.3 !important;
        margin: 0 !important;
        padding: 0 !important;
        width: 100% !important;
        white-space: normal !important; /* Obliga al texto a saltar de línea si no cabe */
        word-wrap: break-word !important;
    }

    /* ==========================================================================
       2. REPARACIÓN DEL MENÚ HAMBURGUESA (ZIGZAG Y BUSCADOR)
       ========================================================================== */
    
    /* Ajuste del contenedor interno (Eliminamos el padding chueco) */
    .wp-block-navigation__responsive-container-content {
        padding: 40px 20px 20px 20px !important; /* Espacio extra arriba para que no choque con la X */
        display: flex !important;
        flex-direction: column !important;
        align-items: center !important; /* Fuerza el centro magnético absoluto */
    }

    /* Reseteo de las listas y submenús (Mata el efecto zigzag) */
    .wp-block-navigation__responsive-container-content ul,
    .wp-block-navigation__responsive-container-content .wp-block-navigation__submenu-container {
        display: flex !important;
        flex-direction: column !important;
        align-items: center !important;
        padding: 0 !important; /* Quita las sangrías automáticas de WordPress */
        margin: 0 !important;
        width: 100% !important;
    }

    /* Ajuste de cada enlace individual */
    .wp-block-navigation__responsive-container-content .wp-block-navigation-item {
        width: 100% !important;
        margin: 0 !important;
        padding: 0 !important;
        display: flex !important;
        justify-content: center !important;
    }

    .wp-block-navigation__responsive-container-content .wp-block-navigation-item a {
        display: block !important; /* Hace que el área táctil sea más grande */
        width: 100% !important;
        text-align: center !important;
        padding: 10px 5px !important; /* Separación vertical entre botones */
        white-space: normal !important; /* Permite que textos largos salten de línea sin cortarse */
        line-height: 1.4 !important;
    }

    /* Arreglo del buscador fantasma (La píldora de abajo) */
    .wp-block-navigation__responsive-container-content .wp-block-search {
        width: 100% !important;
        max-width: 250px !important; /* Para que no se estire a los bordes */
        margin: 20px auto 0 auto !important;
        display: flex !important;
        justify-content: center !important;
    }
    
    .wp-block-navigation__responsive-container-content .wp-block-search__input {
        border: 1px solid #00703c !important; /* Borde verde Wanderers */
        border-radius: 20px !important;
        padding: 8px 15px !important;
        width: 100% !important;
        text-align: center !important; /* Centra el texto "Buscar..." */
        background-color: transparent !important;
    }
}

