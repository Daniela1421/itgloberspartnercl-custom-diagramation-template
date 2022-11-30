# Special Diagramation

Este componente es una grilla interactiva que recibe elementos hijos y permite cambiar el orden desde el site editor.

## Configuration 

### Paso 1 - Clonar

Realizar la [clonación](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) de este repositorio.

### Paso 2 - Editar el Manifest.json 

Ingresar al archivo manifest.json y realizar modificaciones en: `vendor`, `name`, `version`, `title` y `description`
como se muestra en el siguiente ejemplo: 
```
{
  "vendor": "itgloberspartnercl",
  "name": "special-diagramation",
  "version": "0.0.1",
  "title": "Special Diagramation",
  "description": "Grilla interactiva que cambiará un orden y recibirá componentes hijos",
}
```
Además, verifique que el archivo cuente con los siguientes builders: 
```
  "builders": {
    "react": "3.x",
    "messages": "1.x",
    "docs": "0.x",
    "store": "0.x"
  }
```
### Paso 3 - Instalar node-modules

Para realizar esta instalación de node-modules, debe estar ubicado en la carpeta de `react` de la aplicación y ejecutar el comando `yarn`, y tendrá instaladas todas las dependencias necesarias para usar esta plantilla.

### Paso 4 - Ejecutar el preview

Despues de realizar los pasos anteriores puede verificar si su componente está funcionando ejecutando el comando `vtex link` si todo funciona correctamente deberá ver en consola `Sending locale change event`, si por el contrario ocurre un error verifique los pasos anteriores y realice nuevamente este paso. 

### Paso 5 - Implementar el componente

Por último, para utilizar el componente debe agregarlo a las `dependencies` en el `manifest.json` de su tienda de la siguiente manera: vendor.name : version. Por ejemplo: 

```
  "dependencies": {
     "itgloberspartnercl.special-diagramation": "0.x"
  }
```

## Contributors ✨

Daniela Ducuara Cañas
