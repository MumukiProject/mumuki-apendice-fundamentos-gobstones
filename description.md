## Procedimientos Primitivos

### `Poner(color)`

Pone una bolita del color indicado en la casilla actual. Ejemplo: 

```gobstones
program {
  Poner(Rojo) // pone una bolita roja en la casilla actual.
}
```

### `Sacar(color)`

Saca una bolita del color indicado de la casilla actual. Ejemplo: 

```gobstones
program {
  Sacar(Negro) // saca una bolita negra de las que hay en la casilla actual.
}
```

### `Mover(direccion)`

Mueve el cabezal indicador de la casilla actual un paso hacia la dirección indicada. Ejemplo: 

```gobstones
program {
  Mover(Este) // mueve el cabezal una vez hacia el Este.
}
```

### `IrAlBorde(direccion)`

Lleva el cabezal todo lo que se puede hacia la dirección indicada. Ejemplo: 

```gobstones
program {
  IrAlBorde(Norte) // mueve el cabezal de la celda actual a la última celda en la dirección Norte.
}
```

### `VaciarTablero()`

Saca todas las bolitas del tablero, dejando el cabezal en la posición en la que estaba. Ejemplo: 

```gobstones
program {
  VaciarTablero() // En un tablero con alguna o muchas bolitas, las saca todas.
}
```

## Funciones primitivas

### `nroBolitas(color)`

Denota un número: la cantidad de bolitas del color indicado que hay en la casilla actual. Ejemplo, asumiendo la siguiende celda actual: 

![](https://raw.githubusercontent.com/MumukiProject/mumuki-apendice-fundamentos-gobstones/master/sample.png)

```gobstones
nroBolitas(Rojo) // denota 4
```

### `opuesto(direccion)`

Denota una dirección: la dirección opuesta a la provista. Ejemplo:

```gobstones
opuesto(Norte) // denota Sur
```

### `opuesto(numero)`

Denota un número: el original, negado. Ejemplo: 

```gobstenes
opuesto(59) // denota -59
```

### `siguiente(direccion)`

Denota una dirección: la siguiente a la provista, es decir, la próxima en sentido horario. Ejemplo: 

```gobstones
siguiente(Oeste) // denota Norte
siguiente(Norte) // denota Este
siguiente(Este)  // denota Sur
siguiente(Sur)   // denota Sur
```

### `previo(direccion)`

Denota una dirección: la anterior a la provista, es decir, la próxima en sentido anti horario. Ejemplo: 

```gobstones
previo(Sur) // denota Este
```

### `hayBolitas(color)`

Denota un booleano: es cierto cuando en la casilla actual hay al menos una bolita del valor indicado. Ejemplo, asumiendo la siguiende celda actual: 

![](https://raw.githubusercontent.com/MumukiProject/mumuki-apendice-fundamentos-gobstones/master/sample.png)

```gobstones
hayBolitas(Rojo) // denota cierto
hayBolitas(Verde) // denota falso
```

### `puedeMover(direccion)`

Denota un booleano: si el cabezal puede moverse en esa dirección (o sea, no está en el borde). Por ejemplo, estando el cabezal en la esquina de abajo a la izquierda: 

```gobstones
puedeMover(Norte) // denota cierto
puedeMover(Oeste) // denota falso
```

## Expresiones lógicas y matemáticas

* `p ^ q` (_or_): `p && q`
* `p v q` (_and_):  `p || q`
* `¬ p` (_not_):  `not p`
* `x = y` (igual):   `x == y`
* `x ≠ y` (no igual):   `x /= y`
* `x ≥ y` (mayor o igual):   `x >= y`




