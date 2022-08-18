
// Como convertir una web a pwa

1 * Instalar dependencia next-pwa - Crear los iconos de multimedia pwa maskable.app 

- Coger el icono original enmascararlo  en editor - luego voy a load, Coger el icono de galeria organizarlo centrado, y exportar en todos los pixeles descargar

2 * Exportar los logos a la medida - Cambiar los nombres de los iconos y agregarlos a public 

3 * Copiar el manifest que esta en los proyectos terminados y agregar en public, Dentro del código en "name" poner el nombre del proyecto y en "short_name" poner el nombre corto del proyecto,  Generar un archivo favicon.ico 

- Como convertir de png a .icon voy a multimedia convertir png a icon selecionar archivo, Convertir, Descargar, Pegar y poner favicon.ico

4 * Meter el archivo _document.jsx dentro de pages 

5 * Dentro de next.config.js Agregar el siguiente código  de

        //  Usage Without Custom Server (next.js 9+) + add Config 
        const withPWA = require("next-pwa");
        module.exports = withPWA({
        pwa: {
            dest: "public",
            register: true,
            skipWaiting: true,
        },
        });

6 * Antes de ejecutar el proyecto eliminar carpeta .next y hacer un build probarlo con npm start o npm run dev
    Probar que si funciona el PWA - Ejecutamos 

