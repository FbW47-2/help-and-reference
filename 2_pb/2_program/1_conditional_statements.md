# Conditional Statements
Conditional Statments kontrollieren das verhalten von Code in JavaScript, indem sie entscheiden ob Code ausgeführt wird oder nicht.

Es gibt gibt 3 verschiedene Arten von Conditional Statements in Javascript:

- `if`: Wenn die Kondition `true` ergibt, wird der Code innerhalb des "if-Blocks" ausgeführt.
- `else`: Wenn die oben angegebene Kondition `false` ergibtm wird der Code innerhalb des "else-Blocks" ausgeführt.
- `else if`: Wenn auf eine weitere Kondition getestet wird, und die erste kondition fals ist, wird dieser block ausgeführt.

Beispiel:

```js
const testValue = 25;

// If-Statement:
if(testValue > 5)
{
    console.log(`${ testValue } ist größer als 5`);
}
// ergibt: 25 ist größer als 5

// Else-Statement:
if(testValue === 5)
{
    console.log(`${ testValue } ist gleich 5`);
}
else
{
    console.log(`${ testValue } ist nicht 5`);
}
// ergibt: 25 ist nicht 5

// Else-if Statement:
if(testValue === 5)
{
    console.log("testValue ist 5");
}
else if(testValue === 10)
{
    console.log("testValue ist 10");
}
else
{
    console.log("testValue ist eine andere Zahl");
}
// ergibt: testValue ist eine andere zahl
```

## Und, Oder in Conditional-Statements

Um mehrere werte zu vergleichen, kann man einen operator mit in seine if-clause einfügen.
- `||` Der oder Operator
- `&&` Der und Operator
