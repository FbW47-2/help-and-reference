# Loops
Mit loops können wir uns durch listen von einträgen bewegen, um uns informationen ausgeben zu lassen, oder mit den informationen zu arbeiten.

> Ein reales beispiel für einen loop wäre, wenn wir eine Einkaufsliste lesen, und uns jedes einzelne produkt auf der liste genau angucken.

Es gibt mehrere verschiedene Arten von Loops, die für verschiedene anwendungsfälle sinnvoll sind.

## For loop

Der einfache for loop, "die mutter aller loops" hat die komplizierteste syntax, im gegensatz zu den anderen Loops.

Um ihn zu nutzen müssen wir folgende parameter angeben:
- **Initialindex:** wird einmal ausgeführt, bevor der block ausgeführt wird und legt den anfang der iteration fest.
- **Berechnung:** definiert die konditionen zum ausführen des code blocks.
- **Iterator:** wird nach jedem durchlauf des code-blocks ausgeführt und zählt hoch oder runter.

Beispiel:
```js
let counter = 5;

for (let i = 0; i < counter; i++)
{
    console.log(`Hallo Welt!`);
}
```

**Was passiert hier genau?**

| Durchlauf | Variable | Kondition      | Aktion                  |
|-----------|----------|----------------|-------------------------|
| 1         | i = 0    | 0 < 5 == true  | console.log(...); i = 1 |
| 2         | i = 1    | 1 < 5 == true  | console.log(...); i = 2 |
| 3         | i = 2    | 2 < 5 == true  | console.log(...); i = 3 |
| 4         | i = 3    | 3 < 5 == true  | console.log(...); i = 4 |
| 5         | i = 4    | 4 < 5 == true  | console.log(...); i = 5 |
| 6         | i = 5    | 5 < 5 == false | break;                  |

## For/in loop

Der typische weg um durch objekte oder arrays zu loopen ist for/in, dieser loop geht durch verschiedene werte, behält dabei aber nicht zwangsläufig die reihenfolge bei.

Um unsere einträge zu bekommen, nutzen wir innerhalb des code-blocks den namen der array, und dahinter in eckigen klammern (als positionsangabe) den von uns definierten namen des einzelnen eintrages.

```js
const bücherRegal = [ "erstes Buch", "zweites Buch", "drittes Buch", "viertes Buch", "fünftes Buch" ];

for (const buch in bücherRegal)
{
    console.log( bücherRegal[buch] ); // erstes Buch ... 
}

```

## For/of loop
// for/of - loopt durch die verschiedenen werte mit zählbaren inhalt, in der richtigen reihenfolge.
// for/of
// der for-of loop ist etwas neuer und wurde mit ES2015 eingeführt.
// er funktioniert nur mit arrays, da er elemente direkt anspricht und durchgeht, 
// wir können also einfach den variablenamen nutzen:

**Wann nutze ich for/in oder for/of?**

Wie viele andere sachen bei JavaScript könnt ihr auch loops einsetzen wie ihr wollt, und immer wieder damit rumprobieren, aber grundsätlich gilt:

| benutzbar für | for/in | for/off |
|---------------|--------|---------|
| Objekte       | ja     | nein    |
| Arrays        | ja     | ja      |
| Strings       | ja     | ja      |

**Und die performance?!**

Wenn ihr die performance von loops, oder anderen code-schnipsel testen wollt, könnt ihr dies indem über den befehl
```js
console.time("name-des-vergleichs");
```
und unter den code-schnipsel

```js
console.timeEnd("name-des-vergleichs");
```
schreibt. So wird euch in der konsole eine zeitangabe in millisekunden geliefert, die euch sagt wie lang die ausführung vom start zum ende gebraucht hat.

## .forEach();



## while
