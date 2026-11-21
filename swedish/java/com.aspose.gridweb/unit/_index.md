---
title: "Unit"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en längdmätning"
type: docs
url: /sv/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Representerar en längdmätning
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Unit()](#Unit--) | standardkonstruktorn |
| [Unit(double value, int type)](#Unit-double-int-) | Initierar en ny instans av Unit‑strukturen med det angivna dubbelprecision flyttal och UnitType. |
| [Unit(double value)](#Unit-double-) | Initierar en ny instans av Unit‑strukturen med det angivna dubbelprecision flyttal. |
| [Unit(int value)](#Unit-int-) | Initierar en ny instans av Unit‑strukturen med det angivna 32‑bitssignerade heltalet. |
| [Unit(String value)](#Unit-java.lang.String-) | Initierar en ny instans av Unit‑strukturen med den angivna längden. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | hämta sträng efter typ, kan få "px" "pt" "%" och liknande; |
| [Parse(String s)](#Parse-java.lang.String-) | Konverterar den angivna strängen till en Unit. |
| [Percentage(double n)](#Percentage-double-) | Skapar en Unit av typen Percentage från det angivna dubbelprecision flyttalet. |
| [Pixel(int n)](#Pixel-int-) | Skapar en Unit av typen Pixel från det angivna 32‑bitssignerade heltalet. |
| [Point(int n)](#Point-int-) | Skapar en Unit av typen Point från det angivna 32‑bitssignerade heltalet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Hämtar enhetstypen för Unit. |
| [getValue()](#getValue--) | Hämtar längden för Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Hämtar ett värde som indikerar om Unit är tom. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | hämta strängrepresentation av enheten. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


standardkonstruktorn

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Initierar en ny instans av Unit‑strukturen med det angivna dubbelprecision flyttal och UnitType.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |
| typ | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Initierar en ny instans av Unit‑strukturen med det angivna dubbelprecision flyttal.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Initierar en ny instans av Unit‑strukturen med det angivna 32‑bitssignerade heltalet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Initierar en ny instans av Unit‑strukturen med den angivna längden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


hämta sträng efter typ, kan få "px" "pt" "%" och liknande;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Konverterar den angivna strängen till en Unit.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Skapar en Unit av typen Percentage från det angivna dubbelprecision flyttalet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Skapar en Unit av typen Pixel från det angivna 32‑bitssignerade heltalet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Skapar en Unit av typen Point från det angivna 32‑bitssignerade heltalet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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
### getType() {#getType--}
```
public int getType()
```


Hämtar enhetstypen för Unit.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Hämtar längden för Unit.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Hämtar ett värde som indikerar om Unit är tom.

**Returns:**
boolean -
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


hämta strängrepresentation av enheten.

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

