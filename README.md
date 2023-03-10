# week1_day5



## Contenidos

> JS | Data types: objects
>
> JS | Classes
>
> JS | DOM intro & selectors
>
> JS | DOM manipulation


## Main points: objects

- Los objetos de notación literal están compuestos por pares `key: value`

- En relación a las `keys`:
  - Hablamos de una **propiedad** frente a una `key` cuyo valor es cualquier tipo de dato, excepto una función.
  - Hablamos de **método** frente a una `key` cuyo valor es una función.
  
- El acceso a una `key` para hacer un uso _setter_ o _getter_ de la misma, se realiza:
  - Mediante la notación del punto.
  - Mediante el acceso nominal (corchetes).
  
- Las iteraciones aplicables a objetos son:
  - El bucle `for...in` permite recorrer las _keys_ de un objeto.
  - `Object.keys(obj)` permite iterar sobre las _keys_ de un objeto.
  - `Object.values(obj)` permite iterar sobre los valores de un objeto.
  
 - Dentro de método de un objeto la palabra reservada `this`hace referencia al propio objeto.
 
 ## Main points: classes
 
- Las clases describen la estructura que todas sus instancias compartirán.
- Disponen de:
  - **Método constructor**: único, opcional y conectado a la instancia, donde se declaran las propiedades internas de la misma:
    ````javascript
    class Person {
  
      constructor(par1, par2){
          this.propName1 = par1
          this.propName2 = par2
      }
    }
    ````
  - **Métodos prototype**: métodos ordinarios que dotan de capacidades a las instancias.
    ````javascript
    class Person {
  
      methodName(value){
          this.propName += value
      }
    }
    ````
- La palabra reservada `extends` permite extender el alcance inicial de una clase con otra/s clase/s hijas.
- En ellas, el método `super()`permite enviar a la clase padre las propiedades relativas a la misma.

 ## Main points: DOM selectors
 
 - Los selectores DOM permiten alcanzar objetos del documento HTML desde el script:
 
    | Nombre | Argumento | Retorno | Alcance |
    | ------------- | ------------- | ------------- | ------------- |
    | `.querySelector()` | Selector CSS | Nodo | Primer objeto (nodo) que coincida con el selector |
    | `.querySelectorAll()` | Selector CSS | NodeList | Array de objetos (nodos) que coincidan con el selector |
    

- Propiedades principales de los objetos HTML (nodos):
  - `.innerText`
  - `.innerHTML`
  - `.style`
  - `.id`
  - `.className`
  - `.value` para el valor de inputs de formulario

 ## Main points: DOM manipulation
 
 - La manipulación del DOM permite hacer cambios estéticos, de contenido o asociar eventos a objetos del documento mediante:
   - `.removeAttribute()`
   - `.setAttribute()`
   - `.createElement()`
   - `.createTextNode()`
   - `.appendChild()`
   - `.insertBefore()`
   - `.removeChild()`

- Las clases pueden modificarse a través de la propiedad `.classList` y sus métodos `.add()` y `.remove()`
