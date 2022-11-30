# Special Diagramation

Este componente es una grilla interactiva que recibe elementos hijos y permite cambiar el orden desde el site editor.
- Grid 1 
![image](https://user-images.githubusercontent.com/92064924/204862444-e29537e4-e1d1-4992-a444-ab21641bc268.png)
- Grid 2 
![image](https://user-images.githubusercontent.com/92064924/204862673-d9de54d5-3cd9-4bcd-8468-30122cd0fc52.png)
- Grid 3 
![image](https://user-images.githubusercontent.com/92064924/204862458-19050ab5-13d6-4331-a243-993c366f7eb5.png)
- Grid 4 
![image](https://user-images.githubusercontent.com/92064924/204862108-7237e16d-c108-4b68-b66b-f93900772846.png)

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
