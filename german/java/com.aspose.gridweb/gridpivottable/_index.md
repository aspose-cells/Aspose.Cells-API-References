---
title: "GridPivotTable"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt einen PivotTable-Bericht in einem Arbeitsblatt dar."
type: docs
url: /de/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

Stellt einen PivotTable-Bericht in einem Arbeitsblatt dar. Das PivotTable-Objekt ist Mitglied der [GridPivotTable](../../com.aspose.gridweb/gridpivottable)-Sammlung. Die PivotTables‑Sammlung enthält alle PivotTable-Objekte in einer Steuerung.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Fügt das Feld zum spezifischen Bereich hinzu. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Fügt das Feld zum spezifischen Bereich hinzu. |
| [calculateData()](#calculateData--) | Berechnet die Daten der PivotTable in Zellen. |
| [clearAllFields()](#clearAllFields--) | Alle Pivot-Felder löschen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Ruft die spezifischen Felder nach dem Feldtyp ab. |
| [fields(String fieldName)](#fields-java.lang.String-) | Ruft das bestimmte Feld anhand des Feldnamens ab. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Aktualisiert die Daten und Einstellungen der PivotTable aus ihrer Datenquelle. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Fügt das Feld zum spezifischen Bereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Der Typ des Feldbereichs. |
| baseFieldIndex | int | Der Feldindex in den Basisfeldern. |

**Returns:**
int - die Feldposition in den spezifischen Feldern.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Fügt das Feld zum spezifischen Bereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Der Typ des Feldbereichs. |
| fieldName | java.lang.String | Der Name in den Basisfeldern. |

**Returns:**
int - die Feldposition in den spezifischen Feldern. Wenn es kein Feld mit diesem Namen gibt, wird -1 zurückgegeben.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Berechnet die Daten der PivotTable in Zellen.

**Remarks**

Cell.Value im Pivot-Bereich kann kein korrektes Ergebnis zurückgeben, wenn die Methode nicht aufgerufen wurde. Diese Methode berechnet Daten mit einem internen Pivot-Cache, nicht mit der ursprünglichen Datenquelle. Wenn also die Datenquelle geändert wird, rufen Sie bitte zuerst die Methode RefreshData() auf.

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


Alle Pivot-Felder löschen.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


Ruft die spezifischen Felder nach dem Feldtyp ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Der Feldtyp. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


Ruft das bestimmte Feld anhand des Feldnamens ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fieldName | java.lang.String | Der Feldname. |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
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




### refreshData() {#refreshData--}
```
public void refreshData()
```


Aktualisiert die Daten und Einstellungen der PivotTable aus ihrer Datenquelle.

**Remarks**

Wir sammeln Daten aus der Datenquelle in einen Pivot-Cache und berechnen dann die Daten im Cache in die Zellen. Diese Methode wird ausschließlich verwendet, um alle Daten in einen Pivot-Cache zu sammeln.

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

