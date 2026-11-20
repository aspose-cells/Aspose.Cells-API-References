---
title: "PivotFieldGroupSettings"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Gruppeneinstellung des Pivotfelds dar."
type: docs
url: /de/java/com.aspose.cells/pivotfieldgroupsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupSettings
```

Stellt die Gruppeneinstellung des Pivotfelds dar.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // FieldTwo is a data field: move it to the row area first,
         // because only row/column fields can be grouped
         pt.addFieldToArea(PivotFieldType.ROW, "FieldTwo");
         pt.calculateData();
         // Group the numeric field into the ranges 0-1, 2-3, 4-5
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartNumber(0);
         options.setEndNumber(5);
         options.setInterval(2);
         pt.getRowFields().get(1).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputNumberGroupPivotField.xlsx");
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [PivotFieldGroupSettings()](#PivotFieldGroupSettings--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Ermittelt den Gruppentyp des Pivotfelds. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupSettings() {#PivotFieldGroupSettings--}
```
public PivotFieldGroupSettings()
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


Ermittelt den Gruppentyp des Pivotfelds.

Siehe [PivotFieldGroupType](../../com.aspose.cells/pivotfieldgrouptype).

**Returns:**
int
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

