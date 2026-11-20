---
title: "Unit"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt eine Längenmessung dar"
type: docs
url: /de/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Stellt eine Längenmessung dar
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Unit()](#Unit--) | der Standardkonstruktor |
| [Unit(double value, int type)](#Unit-double-int-) | Initialisiert eine neue Instanz der Unit-Struktur mit der angegebenen double-Precision-Gleitkommazahl und UnitType. |
| [Unit(double value)](#Unit-double-) | Initialisiert eine neue Instanz der Unit-Struktur mit der angegebenen double-Precision-Gleitkommazahl. |
| [Unit(int value)](#Unit-int-) | Initialisiert eine neue Instanz der Unit-Struktur mit dem angegebenen 32-bit vorzeichenbehafteten Integer. |
| [Unit(String value)](#Unit-java.lang.String-) | Initialisiert eine neue Instanz der Unit-Struktur mit der angegebenen Länge. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | Hole den String nach dem Typ, kann "px" "pt" "%" und so weiter erhalten; |
| [Parse(String s)](#Parse-java.lang.String-) | Konvertiert den angegebenen String in eine Unit. |
| [Percentage(double n)](#Percentage-double-) | Erstellt eine Unit vom Typ Percentage aus der angegebenen double-Precision-Gleitkommazahl. |
| [Pixel(int n)](#Pixel-int-) | Erstellt eine Unit vom Typ Pixel aus dem angegebenen 32-bit vorzeichenbehafteten Integer. |
| [Point(int n)](#Point-int-) | Erstellt eine Unit vom Typ Point aus dem angegebenen 32-bit vorzeichenbehafteten Integer. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Gibt den Einheitstyp der Unit zurück. |
| [getValue()](#getValue--) | Gibt die Länge der Unit zurück. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Gibt einen Wert zurück, der angibt, ob die Unit leer ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Hole die String‑Repräsentation der Unit. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


der Standardkonstruktor

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Initialisiert eine neue Instanz der Unit-Struktur mit der angegebenen double-Precision-Gleitkommazahl und UnitType.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |
| Typ | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Initialisiert eine neue Instanz der Unit-Struktur mit der angegebenen double-Precision-Gleitkommazahl.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Initialisiert eine neue Instanz der Unit-Struktur mit dem angegebenen 32-bit vorzeichenbehafteten Integer.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Initialisiert eine neue Instanz der Unit-Struktur mit der angegebenen Länge.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


Hole den String nach dem Typ, kann "px" "pt" "%" und so weiter erhalten;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Konvertiert den angegebenen String in eine Unit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Erstellt eine Unit vom Typ Percentage aus der angegebenen double-Precision-Gleitkommazahl.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Erstellt eine Unit vom Typ Pixel aus dem angegebenen 32-bit vorzeichenbehafteten Integer.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Erstellt eine Unit vom Typ Point aus dem angegebenen 32-bit vorzeichenbehafteten Integer.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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


Gibt den Einheitstyp der Unit zurück.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Gibt die Länge der Unit zurück.

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


Gibt einen Wert zurück, der angibt, ob die Unit leer ist.

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


Hole die String‑Repräsentation der Unit.

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

