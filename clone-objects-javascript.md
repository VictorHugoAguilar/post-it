Ya que los objetos en javascript son valores por referencia, no pueden copiarse simplemente con el =. Aqui os dejo diferentes maneras de hacerlo.
 
```
let profesiones = { medico: '🚑', policia: '🚓', bombero: '🚒' }

// "Spread operator"
let clone_one = { ...profesiones }
console.log(clone_one) 
// clone_one { medico: '🚑', policia: '🚓', bombero: '🚒' }

// "Object.assign
let clone_two = Object.assign({}, profesiones)
console.log(clone_two) 
// clone_two { medico: '🚑', policia: '🚓', bombero: '🚒' }

// "JSON"
let clone_three = JSON.parse(JSON.stringify(profesiones))
console.log(clone_three) 
// clone_three { medico: '🚑', policia: '🚓', bombero: '🚒' }
```

## Los objetos son tipo referencia

