# Datos curiosos
![](http://www.cursosgis.com/wp-content/uploads/2017/06/lenguajes_1.png)
**Tabla de contenidos**

[TOCM]

[TOC]
##Programación en general
###Editores de texto
+ Los editores de código: Se centran en `distintos lenguajes, a nivel sencillo.` Se pueden potenciar con extensiones para simular IDE's
+ Los IDE's se centran en `un lenguaje a nivel de proyecto.`
### Manejo de proyectos
+ En proyectos grandes, es complicado mantener un ambiente virtual. Divide y vencerás es partir un problema difícil en partes pequeñas. Cada paquete se desarrolla a su propio ritmo (no siempre preocupándose de la compatibilidad con otros módulos). 
+ Hay tres tipos de paquetes: Externos, Modelo y de Comunicación. Entonces podemos crear en multiples ambientes en un solo proyecto.  Para esto, creamos una carpeta llamada envs y creamos tres documentos: external.yml, model.yml y comunicacion.yml.
+ Snakemake es un paquete que implementa muy bien este concepto. Es un motor de workflows . Cada paso lo ejecuta con un ambiente específico.
##HTML
+ El atriputo name de input hace referencia al grupo de inputs
+ El atributo for, fusiona un label con un input si tienen el mismo nombre
##CSS
+ overflow-x: `establece lo que se muestra cuando el contenido desborda los bordes` izquierdo y derecho de un elemento a nivel de bloque. Puede que no sea nada, una barra de desplazamiento o el contenido adicional.
+ overscroll-behavior: `establece lo que hace un navegador cuando alcanza el límite de un área de desplazamiento`. Es un abreviatura de overscroll-behavior-x overscroll-behavior-y
+ scroll-snap-type: `establece qué tan estrictamente se aplican los puntos de snap en el contenedor de desplazamietno en caso de que haya uno.`
+ `object-fit: cover` hace que una imagen no se vea contraida, mantendrá su tamaño sin depender de nadd
####Slide fácil:
```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Hello world!</title>
    </head>
	<style>
        .contenedor-padre{
            display: flex;
            overflow-x: scroll;
            overscroll-behavior-x: contain;
            scroll-snap-type: proximity;
        }
        .contenedor-hijo{
            scroll-snap-align: center;
        }
	</style>
    <body>
        <h1>Slide fácil</h1>
		<div class="contenedor-padre">
            <div class="contenedor-hijo">
		<p>Aquí van los contenedores</p>
            </div>   
		</div>
    </body>
</html>
```
####Centrar elementos vertical y horizontalmente
```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <title>Hello world!</title>
    </head>
	<style>
        .contenedor-padre{
            display:grid;
			place-items:center;
        }
	</style>
    <body>
        <h1>Slide fácil</h1>
		<div class="contenedor-padre">
            <div class="contenedor-hijo">
				<p>Aquí van los contenedores</p>
            </div>   
		</div>
    </body>
</html>
```

##JS
+ Si en un if else queremos que se ejecute una sentencia y después no pase nada más, le colocamos return
+ ```javascript 
	console.warmn("a") /*Warning*/
		```
###Imprimir cada elemento de un array
```javascript
function imprimirElementoxElemento(arr){
	for(let i = 0; i < arr.length,;i++){
		console.log(arr[i])
	}
}
```
###Imprimir todos los elementos de un array
```javascript
	console.log(Object.entries(object));
```

###Var vs Let vs Const
![](https://pbs.twimg.com/media/EeVw-DOXgAAMtKk.jpg)
###Parámetros y argumentos de una función
![](https://preview.redd.it/bxkz9iko0u681.png?auto=webp&s=dfcf8222d495f9c71bc5b5fb17468b33e7cba0e9)
----
