# Datos curiosos

![](http://www.cursosgis.com/wp-content/uploads/2017/06/lenguajes_1.png)



**Tabla de contenidos**

[TOCM]

[TOC]
##Programación en general
+ Los editores de código: Se centran en distintos lenguajes, a nivel sencillo, se pueden potenciar con extensiones para simular IDE's
+ Los IDE's se centran en un lenguaje a nivel de proyecto.
##HTML
+ El atriputo name de input hace referencia al grupo de inputs
+ El atributo for, fusiona un label con un input
##CSS
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

#JS

----
