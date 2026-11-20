---
title: "CalculationPrecisionStrategy"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Enumera le strategie per gestire la precisione del calcolo."
type: docs
url: /it/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

Elenca le strategie per gestire la precisione dei calcoli. A causa del problema di precisione dell'aritmetica a virgola mobile IEEE 754, alcune formule \"apparente semplici\" potrebbero non essere calcolate come il risultato previsto. Ad esempio la formula \"=-0.45+0.43+0.02\", calcolando gli operandi con l'operatore '+' direttamente, il risultato non è zero. Per questo tipo di problema di precisione, alcune strategie speciali possono fornire il risultato atteso.
## Campi

| Campo | Descrizione |
| --- | --- |
| [DECIMAL](#DECIMAL) | Utilizza il decimale come operando quando possibile. |
| [NONE](#NONE) | Nessuna strategia applicata al calcolo. |
| [ROUND](#ROUND) | Arrotonda il risultato del calcolo in base alle cifre significative. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Utilizza i decimali come operandi quando possibile. Molto inefficiente per le prestazioni.

### NONE {#NONE}
```
public static final int NONE
```


Nessuna strategia applicata al calcolo. Durante il calcolo utilizza semplicemente il valore double originale come operando e restituisce direttamente il risultato. Molto efficiente per le prestazioni e applicabile nella maggior parte dei casi.

### ROUND {#ROUND}
```
public static final int ROUND
```


Arrotonda il risultato del calcolo in base alle cifre significative.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

