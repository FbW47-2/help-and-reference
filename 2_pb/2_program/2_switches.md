# Switches
Ein switch kann mehrere blocks mit code ausführen, und kann außerdem, wenn keine Kondition eintrifft, auf einen default code-block springen.

## Wozu dient break;?

Wenn ein `break;` Kommando erreicht wurde, verlässt JavaScript den Switch und führt den rest des Codes aus. Das letzte Switch-Statement benötigt kein `break;` Kommando, da danach ohnehin der Switch verlassen wird.

## Wie vergleicht ein switch?

Switches vergleichen werte in strikter form, also in form des `===`:

Beispiel:
```js
const testValue = "0";

switch (testValue) {
  case 0:
    console.log("Off");
    break;
  case 1:
    console.log("On");
    break;
  default:
    console.log("No value found");
}
// ergibt: "No Value Found";
```
