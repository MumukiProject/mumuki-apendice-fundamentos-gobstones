# Procedimientos Primitivos

## `Poner(color)`

> Pone una bolita del color indicado en la casilla actual

Ejemplo: 

```gobstones
program {
  Poner(Rojo) // pone una bolita roja en la casilla actual.
}
```

## `Sacar(color)`

> Saca una bolita del color indicado de la casilla actual

Ejemplo: 

```gobstones
program {
  Sacar(Negro) // saca una bolita negra de las que hay en la casilla actual.
}
```

## `Mover(direccion)`

> Mueve el cabezal indicador de la casilla actual un paso hacia la dirección indicada.

Ejemplo: 

```gobstones
program {
  Mover(Este) // mueve el cabezal una vez hacia el Este.
}
```

## `IrAlBorde(direc)`

> Lleva el cabezal todo lo que se puede hacia la dirección indicada

Ejemplo: 

```gobstones
program {
  IrAlBorde(Norte) // mueve el cabezal de la celda actual a la última celda en la dirección Norte.
}
```

## `VaciarTablero()`

> Saca todas las bolitas del tablero, dejando el cabezal en la posición en la que estaba.

Ejemplo: 

```gobstones
program {
  VaciarTablero() // En un tablero con alguna ó muchas bolitas, las saca todas.
}
```
