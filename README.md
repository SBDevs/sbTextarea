# sbTextarea

Directiva de AngularJS que amplia la funcionalidad y compatibilidad del <textarea></textarea>.
Esta directiva ha sido creada para que sea compatible con la mayoria de los navegadores (especialmente con IE y Chrome).

### Como empezar

Debe descargar el proyecto donde encontrará todo lo necesario para usar estas directivas.  

### Prerequisito

Para usar sb-textarea, necesitas implementar AngularJS en su solución web. 
Se hace uso de bootstrap y fontawesome, ya que son ampliamente utilizadas en el desarrollo web. 

## Atributos

Esta directiva contiene los siguientes atributos en su definicion:

| Atributo    | Definición                                                           |
|:-----------:|:--------------------------------------------------------------------:|
| contenido   | Valor con el que se va a trabajar en el control                      |
| longitud    | Numero de caracteres que se pueden rellenar                                             |
| limitacion  | Si es true, cuando el numero de caracteres llegue a la longitud, no podrás seguir escribiendo. En caso contrario de avisara pero podras seguir escribiendo |
| altura      | Numero de lineas que se mostrarán en el area | 

## Ejemplos

### html

```html
 <div id="CapaDemoDirectivas" ng-controller="CtlDemoDirectivas">
 ...
 </div>
```

```html
<sb-textarea contenido="Nombre" longitud="10" limitacion="false" altura="2"></sb-textarea>
```

```html
<sb-textarea id="t1" longitud="5" limitacion="true" altura="4"></sb-textarea>
```

### JavaScript 

```javascript
var appDemoDirectivas = angular.module('appDemoDirectivas', ['Directivas']);

var CtlDemoDirectivas = function ($scope) {
	$scope.Nombre = "";
};

CtlDemoDirectivas.$inject = ['$scope'];

appDemoDirectivas.controller('CtlDemoDirectivas', CtlDemoDirectivas);

var CapaDemoDirectivas = document.getElementById('CapaDemoDirectivas');
angular.bootstrap(CapaDemoDirectivas, ['appDemoDirectivas']);

```
Ejemplos en [http://sbcontrols.ml/](http://sbcontrols.ml/) 

## Herramientas utilizadas

  * [AngularJs](https://angularjs.org/)
  * [BootStrap](http://getbootstrap.com/getting-started/)
  * [FontAwesome](http://fontawesome.io/)	

## Autores

Esta directiva ha sido desarrollado como trabajo para la asignatura SOFTWARE LIBRE Y COMPROMISO SOCIAL de la Universidad de Córdoba.

El desarrollador principal de esta directiva 

```
Eloy Ortiz Pulido
```

Desarrolladores del resto de directivas sb-controls

```
Verónica Gómez Molina
Manuel David Ruiz Rubio
``` 

Especial agradecimiento por sus masterclass en angularjs

```
Rafael Torres Cabezas
```
