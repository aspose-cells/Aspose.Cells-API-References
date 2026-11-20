---
title: "SheetSet"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Beschreibt eine Menge von Blättern."
type: docs
url: /de/java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

Beschreibt eine Menge von Blättern.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SheetSet(int[] sheetIndexes)](#SheetSet-int---) | Erstellt ein Blattset basierend auf genauen Blattindizes. |
| [SheetSet(String[] sheetNames)](#SheetSet-java.lang.String---) | Erstellt ein Blattset basierend auf genauen Blattnamen. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Gibt ein Set mit dem aktiven Blatt der Arbeitsmappe zurück. |
| [getAll()](#getAll--) | Gibt ein Set mit allen Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge zurück. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Gibt ein Set mit sichtbaren Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge zurück. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheetIndexes) {#SheetSet-int---}
```
public SheetSet(int[] sheetIndexes)
```


Erstellt ein Blattset basierend auf genauen Blattindizes.

**Remarks**

Wenn ein Blatt gefunden wird, das nicht in der Arbeitsmappe enthalten ist, wird beim Rendern eine Ausnahme ausgelöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndexes | int[] | Nullbasierte Blattindizes. |

### SheetSet(String[] sheetNames) {#SheetSet-java.lang.String---}
```
public SheetSet(String[] sheetNames)
```


Erstellt ein Blattset basierend auf genauen Blattnamen.

**Remarks**

Wenn ein Blatt gefunden wird, das nicht in der Arbeitsmappe enthalten ist, wird beim Rendern eine Ausnahme ausgelöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetNames | java.lang.String[] | Blattnamen. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Gibt ein Set mit dem aktiven Blatt der Arbeitsmappe zurück.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Gibt ein Set mit allen Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge zurück.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Gibt ein Set mit sichtbaren Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge zurück.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

