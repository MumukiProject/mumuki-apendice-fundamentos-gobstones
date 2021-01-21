<ul>

<li><a title="" href="#procedimientos-primitivos">Procedimientos Primitivos</a>
<ul>
<li><a title="" href="#ponercolor"><code>Poner(color)</code></a></li>
<li><a title="" href="#sacarcolor"><code>Sacar(color)</code></a></li>
<li><a title="" href="#moverdireccion"><code>Mover(direccion)</code></a></li>
<li><a title="" href="#iralbordedireccion"><code>IrAlBorde(direccion)</code></a></li>
<li><a title="" href="#vaciartablero"><code>VaciarTablero()</code></a></li>
</ul>
</li>


<li><a title="" href="#funciones-primitivas">Funciones primitivas</a>
<ul>
<li><a title="" href="#nrobolitascolor"><code>nroBolitas(color)</code></a></li>
<li><a title="" href="#opuestodireccion"><code>opuesto(direccion)</code></a></li>
<li><a title="" href="#opuestonumero"><code>opuesto(numero)</code></a></li>
<li><a title="" href="#siguientedireccion"><code>siguiente(direccion)</code></a></li>
<li><a title="" href="#previodireccion"><code>previo(direccion)</code></a></li>
<li><a title="" href="#haybolitascolor"><code>hayBolitas(color)</code></a></li>
<li><a title="" href="#puedemoverdireccion"><code>puedeMover(direccion)</code></a></li>
</ul>
</li>
<li><a title="" href="#expresiones-logicas-y-matematicas">Expresiones lógicas y matemáticas</a>


<h2 id="procedimientos-primitivos">Procedimientos Primitivos</h2>

<a id="ponercolor"></a>
### `Poner(color)`

Pone una bolita del color indicado en la casilla actual. Ejemplo: 

```gobstones
program {
  Poner(Rojo) // pone una bolita roja en la casilla actual.
}
```

<a id="sacarcolor"></a>
### `Sacar(color)`

Saca una bolita del color indicado de la casilla actual. Ejemplo: 

```gobstones
program {
  Sacar(Negro) // saca una bolita negra de las que hay en la casilla actual.
}
```

<a id="moverdireccion"></a>
### `Mover(direccion)`

Mueve el cabezal indicador de la casilla actual un paso hacia la dirección indicada. Ejemplo: 

```gobstones
program {
  Mover(Este) // mueve el cabezal una vez hacia el Este.
}
```

<a id="iralbordedireccion"></a>
### `IrAlBorde(direccion)`

Lleva el cabezal todo lo que se puede hacia la dirección indicada. Ejemplo: 

```gobstones
program {
  IrAlBorde(Norte) // mueve el cabezal de la celda actual a la última celda en la dirección Norte.
}
```

<a id="vaciartablero"></a>
### `VaciarTablero()`

Saca todas las bolitas del tablero, dejando el cabezal en la posición en la que estaba. Ejemplo: 

```gobstones
program {
  VaciarTablero() // En un tablero con alguna o muchas bolitas, las saca todas.
}
```

<h2 id="funciones-primitivas">Funciones primitivas</h2>

<a id="nrobolitascolor"></a>
### `nroBolitas(color)`

Denota un número: la cantidad de bolitas del color indicado que hay en la casilla actual. Ejemplo, asumiendo la siguiende celda actual: 

![](https://raw.githubusercontent.com/MumukiProject/mumuki-apendice-fundamentos-gobstones/master/sample.png)

```gobstones
nroBolitas(Rojo) // denota 4
```

<a id="opuestodireccion"></a>
### `opuesto(direccion)`

Denota una dirección: la dirección opuesta a la provista. Ejemplo:

```gobstones
opuesto(Norte) // denota Sur
```

<a id="opuestonumero"></a>
### `opuesto(numero)`

Denota un número: el original, negado. Ejemplo: 

```gobstenes
opuesto(59) // denota -59
```

<a id="siguientedireccion"></a>
### `siguiente(direccion)`

Denota una dirección: la siguiente a la provista, es decir, la próxima en sentido horario. Ejemplo: 

```gobstones
siguiente(Oeste) // denota Norte
siguiente(Norte) // denota Este
siguiente(Este)  // denota Sur
siguiente(Sur)   // denota Sur
```

<a id="previodireccion"></a>
### `previo(direccion)`

Denota una dirección: la anterior a la provista, es decir, la próxima en sentido anti horario. Ejemplo: 

```gobstones
previo(Sur) // denota Este
```

<a id="haybolitascolor"></a>
### `hayBolitas(color)`

Denota un booleano: es cierto cuando en la casilla actual hay al menos una bolita del valor indicado. Ejemplo, asumiendo la siguiende celda actual: 

![](https://raw.githubusercontent.com/MumukiProject/mumuki-apendice-fundamentos-gobstones/master/sample.png)

```gobstones
hayBolitas(Rojo) // denota cierto
hayBolitas(Verde) // denota falso
```

<a id="puedemoverdireccion"></a>
### `puedeMover(direccion)`

Denota un booleano: si el cabezal puede moverse en esa dirección (o sea, no está en el borde). Por ejemplo, estando el cabezal en la esquina de abajo a la izquierda: 

```gobstones
puedeMover(Norte) // denota cierto
puedeMover(Oeste) // denota falso
```

<h2 id="expresiones-logicas-y-matematicas">Expresiones lógicas y matemáticas</h2>

* `p ^ q` (_or_): `p && q`
* `p v q` (_and_):  `p || q`
* `¬ p` (_not_):  `not p`
* `x = y` (igual):   `x == y`
* `x ≠ y` (no igual):   `x /= y`
* `x ≥ y` (mayor o igual):   `x >= y`
