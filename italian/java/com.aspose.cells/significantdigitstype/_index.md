---
title: "SignificantDigitsType"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il tipo di cifre significative per l'emissione di valori numerici."
type: docs
url: /it/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Rappresenta il tipo di cifre significative per l'emissione di valori numerici.
## Campi

| Campo | Descrizione |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15 cifre |
| [G_17](#G-17) | 17 cifre formattando il valore con "G17". |
| [ROUNDING_17](#ROUNDING-17) | 17 cifre arrotondando il valore. |
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
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15 cifre

### G_17 {#G-17}
```
public static final int G_17
```


17 cifre formattando il valore con "G17".

**Remarks**

Per alcuni valori double, "G17" può fornire un valore diverso da quello originale/litterale inserito dall'utente. Per esempio, il valore double 0.15 verrà restituito come 0.14999999999999999; il valore double 1.0E-16 verrà restituito come 9.9999999999999998E-17. Excel gestisce questi valori in modo incoerente: salva 0.15 come 0.15 nel file xlsx, ma per 1.0E-16 il valore salvato nel file xlsx è 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17 cifre arrotondando il valore.

**Remarks**

Questo tipo generalmente restituisce il valore così com'era originale/litterale inserito dall'utente. Per 0.15 produce "0.15" e per 1.0E-16 produce "1.0E-16". Tuttavia ci sono anche alcuni casi speciali che possono dare valori diversi dal litterale. Per esempio, arrotondando 208435494.96478021 a 17-cifre("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#"), l'output è 208435494.96478.

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

