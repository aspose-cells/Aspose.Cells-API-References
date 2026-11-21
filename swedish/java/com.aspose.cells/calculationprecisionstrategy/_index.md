---
title: "CalculationPrecisionStrategy"
second_title: "Aspose.Cells för Java API-referens"
description: "Enumererar strategier för hantering av beräkningsprecision."
type: docs
url: /sv/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

Enumererar strategier för att hantera beräkningsprecision. På grund av precisionsproblemet i IEEE 754 flyttalsaritmetik kan vissa \"till synes enkla\" formler inte beräknas till det förväntade resultatet. Till exempel formeln \"=-0.45+0.43+0.02\", när operander beräknas med '+'-operatorn direkt, blir resultatet inte noll. För den här typen av precisionsproblem kan vissa speciella strategier ge det förväntade resultatet.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [DECIMAL](#DECIMAL) | Använder decimal som operander när det är möjligt. |
| [NONE](#NONE) | Ingen strategi tillämpas på beräkning. |
| [ROUND](#ROUND) | Avrundar beräkningsresultatet enligt signifikanta siffror. |
## Metoder

| Metod | Beskrivning |
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


Använder decimal som operander när det är möjligt. Mest ineffektiv för prestanda.

### NONE {#NONE}
```
public static final int NONE
```


Ingen strategi tillämpas på beräkning. Vid beräkning används bara det ursprungliga double‑värdet som operand och resultatet returneras direkt. Mest effektiv för prestanda och tillämplig i de flesta fall.

### ROUND {#ROUND}
```
public static final int ROUND
```


Avrundar beräkningsresultatet enligt signifikanta siffror.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

