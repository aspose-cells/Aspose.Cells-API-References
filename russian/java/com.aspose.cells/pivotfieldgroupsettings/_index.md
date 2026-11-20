---
title: "PivotFieldGroupSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройку группы сводного поля."
type: docs
url: /ru/java/com.aspose.cells/pivotfieldgroupsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupSettings
```

Представляет настройку группы сводного поля.

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
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [PivotFieldGroupSettings()](#PivotFieldGroupSettings--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Получает тип группы сводного поля. |
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
| Параметр | Тип | Описание |
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


Получает тип группы сводного поля.

Смотрите [PivotFieldGroupType](../../com.aspose.cells/pivotfieldgrouptype).

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

