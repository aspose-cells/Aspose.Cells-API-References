---
title: "CustomFunctionDefinition"
second_title: "Aspose.Cells för Java API-referens"
description: "Definition av anpassad funktion för beräkning med användarens anpassade motor."
type: docs
url: /sv/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

Definition av anpassad funktion för beräkning med användarens anpassade motor.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | Hämtar index för den angivna anpassade funktionens parametrar som måste beräknas i arrayläge. |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


Hämtar index för den angivna anpassade funktionens parametrar som måste beräknas i arrayläge.

**Remarks**

För ett uttryck som måste beräknas, med A:A+B:B som exempel: Vanligtvis i värdeläge beräknas det till ett enda värde enligt den aktuella cellbasen. Men i arrayläge beräknas alla värden av A1+B1, A2+B2, A3+B3, … och används för beräkningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| functionName | java.lang.String | Namn på den anpassade funktionen. |

**Returns:**
int[] – Index för de parametrar som måste beräknas i arrayläge för den angivna anpassade funktionen. Standard är null, det finns ingen parameter som måste beräknas i arrayläge för den anpassade funktionen.
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

