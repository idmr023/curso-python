#Curso básico de JS
##Arrays:
```javascript

var frutas = ["Manzana","Pera","Cereza"];

var masFrutas = frutas.push("Uvas"); //Para agregar elementos al final del array
var ultimo = frutas.pop("Uvas"); //Para eliminar elementos al final del array
var nuevaLongitud = frutas.unshift("Plátano") //Para agregar elementos al inicio del array
var borrarLongitud = frutas.shift("Melón") //Para eliminar elementos al inicio del array
var borrarLongitud2 = frutas.splice(2,1) //Para eliminar elementos según el índice. El primer parámetro es el índice y el segundo cuantos elementos se eliminan
var posicion = frutas.indexOf("Cereza"); //Para saber la ubicación, en el array, de un elemento


//Recorrer arrays

var articulos  = [
    { nombre: "Bici", costo: 300 }, 
    { nombre: "TV", costo: 5500 },
    { nombre: "Libro", costo: 50 },
    { nombre: "Celular", costo: 750 },
    { nombre: "Laptop", costo: 4500 },
    { nombre: "Teclado", costo: 250 },
    { nombre: "Audífonos", costo: 50 }
];

//Primera forma. Crea un nuevo array con los elementos del array que se pasó como parámetro y que cumplan con la condición definida.
var articulosFiltrados = articulos.filter(function(articulo){
    return articulo.costo >= 5000 
 });

//Segunda forma. Crea un nuevo array con los resultados de la llamada a la función indicada aplicados a cada uno de sus elementos.
var nombreArticulos = articulos.map(function(articulo){
	return articulo.nombre
});

//Tercera forma. Retorna el primer elemento de un array que cumple con una condición definida en un nuevo array.
var encuentraArticulo = articulos.find(function(articulo){
    return articulo.nombre === 'Laptop'
});

//Cuarta forma. Ejecuta la función indicada una vez por cada elemento del array.
articulos.forEach(function(articulo){
    console.log(articulo.nombre);
});

//Quinta forma. Retorna "true"o “false” si hay elementos en un array que cumplan con la condición indicada.
var articulosBaratos = articulos.some(function(articulo){
    return articulo.costo <= 700;
});

```
