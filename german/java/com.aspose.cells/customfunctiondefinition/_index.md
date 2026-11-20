---
title: "CustomFunctionDefinition"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Definition einer benutzerdefinierten Funktion für Berechnungen mit der benutzerdefinierten Engine des Benutzers."
type: docs
url: /de/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

Definition einer benutzerdefinierten Funktion zur Berechnung mit der benutzerdefinierten Engine des Benutzers.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | Ruft die Indizes der Parameter der angegebenen benutzerdefinierten Funktion ab, die im Array‑Modus berechnet werden müssen. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


Ruft die Indizes der Parameter der angegebenen benutzerdefinierten Funktion ab, die im Array‑Modus berechnet werden müssen.

**Remarks**

Für einen Ausdruck, der berechnet werden muss, am Beispiel A:A+B:B: In der Regel wird er im Wertmodus zu einem einzelnen Wert basierend auf der aktuellen Zellenbasis berechnet. Im Array‑Modus hingegen werden alle Werte von A1+B1, A2+B2, A3+B3, … berechnet und für die Berechnung verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| functionName | java.lang.String | Name der benutzerdefinierten Funktion. |

**Returns:**
int[] – Indizes der Parameter, die für die angegebene benutzerdefinierte Funktion im Array‑Modus berechnet werden müssen. Standardwert ist null, es gibt keinen Parameter, der im Array‑Modus berechnet werden muss.
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

