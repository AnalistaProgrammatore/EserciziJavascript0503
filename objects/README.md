## ESERCIZI OGGETTI

1. Scrivi nel file `hello.js` il codice javascript che esegue i seguenti step
  - crea un oggetto `user` vuoto
  - aggiunge una proprietà `name` con i flag di default e valore `Mario`
  - aggiunge una proprietà `surname` con i flag `writeable: false` e `configurable: false` con valore `Rossi`
  - modifica il valore della proprietà `name` al valore `Marco`
  - elimina la proprietà `name` dall'oggetto `user`

2. Scrivi nel file `isEmpty.js` la funzione `iseEmpty` che dato un oggetto in input ritorni `true` se l'oggetto è vuoto e `false` altrimenti

3. Dato il seguente oggetto 
```
let salaries = {
  John: 100,
  Ann: 160,
  Pete: 130
}
```
Scrivere nel file `salaries.js` la funzione `sumSalaries` che dato in input l'oggetto `salaries` produca in output la somma di tutti i salari contenuti

4. Scrivi nel file `multiply.js` una funzione `multiply` che dato in input un oggetto e un numero moltiplichi tutte le proprietà numeriche dell'oggetto per il numero dato. NB la funzione deve essere pura. Ad esempio
```
let menu = {
  width: 200,
  height: 300,
  title: "My menu"
}

const newMenu = multiplyNumeric(menu, 2)

// after the call
newMenu = {
  width: 400,
  height: 600,
  title: "My menu"
}
```
5. creare nel file `calculator.js` un oggetto `calculator` con una proprietà `values`: un array di valori e 4 metodi `add`, `sub`, `mul`, `div` che eseguano le 4 operazioni fondamentali sulla proprietà `values` e restituiscano in output il risultato dell'operazione. Ad esempio:
```
let calculator = {
  // ... your code ...
}

calculator.values = [...];
console.log( calculator.sum() )
console.log( calculator.sub() )
console.log( calculator.mul() )
console.log( calculator.div() )
```
NB gestire il caso della divisione per 0
NB usate il metodo `reduce` degli array per ottenre i risultati dei vari metodi

6. Dato il seguente codice:
```
let ladder = {
  step: 0,
  up() {
    this.step++
  },
  down() {
    this.step--
  },
  showStep: function() { // shows the current step
    console.log( this.step )
  }
}
ladder.up()
ladder.up()
ladder.down()
ladder.showStep() // 1
```
riscriverlo nel file `chaining.js` in modo che possa funzionare nel seguente modo cioè usando il `method chaining`:
```
ladder.up().up().down().showStep() // 1
```
7. creare nel file `calculatorConstructor.js` la funzione costrutture `Calculator(values)` che dato in input un array di valori crei l'oggetto `calculator` dell'esercizio numero 5.
```
let calculator = new Calculator([...]);

console.log( calculator.sum() )
console.log( calculator.sub() )
console.log( calculator.mul() )
console.log( calculator.div() )
```
