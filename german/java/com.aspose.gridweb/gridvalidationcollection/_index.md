---
title: "GridValidationCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt eine Sammlung von Objekten."
type: docs
url: /de/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

Kapselt eine Sammlung von [GridValidation](../../com.aspose.gridweb/gridvalidation)-Objekten.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add()](#add--) | Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Fügt der Sammlung eine Datenvalidierung hinzu. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu. |
| [add(int row, int column)](#add-int-int-) | Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu. Die Validierung wird auf die angegebene Zelle angewendet. |
| [add(String cellname)](#add-java.lang.String-) | Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu. Die Validierung wird auf die angegebene Zelle angewendet. |
| [clear()](#clear--) | Löscht alle Validierungen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ruft das [GridValidation](../../com.aspose.gridweb/gridvalidation)-Element am angegebenen Index ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Größe des Enumerators ab. |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Ruft die auf die angegebene Zelle angewendete Validierung ab. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt die Validierung am angegebenen Index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode GridValidationCollection.Add(row,col). Diese Eigenschaft wird 12 Monate nach JANUAR 2015 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


Fügt der Sammlung eine Datenvalidierung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Der Bereich enthält diese Validierung. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | Ein Validierungsobjekt. |

**Returns:**
int - Index des [GridValidation](../../com.aspose.gridweb/gridvalidation)-Objekts.
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu. Die Validierung wird auf die angegebene Zelle angewendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


Fügt ein [GridValidation](../../com.aspose.gridweb/gridvalidation) zur Sammlung hinzu. Die Validierung wird auf die angegebene Zelle angewendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellname | java.lang.String | Der Name der Zelle. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


Löscht alle Validierungen.

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
### get(int index) {#get-int-}
```
public GridValidation get(int index)
```


Ruft das [GridValidation](../../com.aspose.gridweb/gridvalidation)-Element am angegebenen Index ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ruft die Größe des Enumerators ab.

**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


Ruft die auf die angegebene Zelle angewendete Validierung ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Der Zeilenindex. |
| Spalte | int | Der Spaltenindex. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Entfernt die Validierung am angegebenen Index.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Der nullbasierte Index des Elements. |

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

