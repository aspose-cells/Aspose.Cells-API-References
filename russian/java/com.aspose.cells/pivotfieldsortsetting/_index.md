---
title: "PivotFieldSortSetting"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройку сортировки сводных полей."
type: docs
url: /ru/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

Представляет настройку сортировки сводных полей.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Sort by the first data field ascending.
         rowField.sortBy(SortOrder.ASCENDING, 0, null);
 
         //Gets sort settings of the pivot field.
         PivotFieldSortSetting sortSetting = rowField.getSortSetting();
         System.out.println(sortSetting.getSortType());
         //do your business
 
         pivot.calculateData();
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Сортирует по значениям в строке или столбце. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | Представляет индекс поля, по которому производится сортировка. |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | Тип строки сводки, по которому производится сортировка. |
| [getSortBy()](#getSortBy--) | Представляет индекс поля, по которому производится сортировка. |
| [getSortType()](#getSortType--) | Представляет [SortOrder](../../com.aspose.cells/sortorder). |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | Указывает, будет ли применена простая операция сортировки данных. |
| [isSortByLabels()](#isSortByLabels--) | Указывает, сортировать ли поле само по себе или по полю данных. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | Представляет индекс поля, по которому производится сортировка. |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | Указывает, будет ли применена простая операция сортировки данных. |
| [setSortBy(int value)](#setSortBy-int-) | Представляет индекс поля, по которому производится сортировка. |
| [setSortType(int value)](#setSortType-int-) | Представляет [SortOrder](../../com.aspose.cells/sortorder). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCell() {#getCell--}
```
public String getCell()
```


Сортирует по значениям в строке или столбце.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Представляет индекс поля, по которому производится сортировка. -1 означает сортировку PivotField по меткам, остальные значения означают сортировку по полю данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotFieldSortSetting.SortBy. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


Тип строки сводки, по которому производится сортировка.

См. [PivotLineType](../../com.aspose.cells/pivotlinetype).

**Remarks**

Работает только когда это поле не сортируется по меткам.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


Представляет индекс поля, по которому производится сортировка. Значение -1 указывает на сортировку по собственным значениям элемента сводки. При значении, большем или равном нулю, представляет индекс поля данных в области данных.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


Представляет [SortOrder](../../com.aspose.cells/sortorder).

См. [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSimpleSort() {#isSimpleSort--}
```
public boolean isSimpleSort()
```


Указывает, будет ли применена простая операция сортировки данных.

**Remarks**

Значение по умолчанию — true.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


Указывает, сортировать ли поле само по себе или по полю данных.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


Представляет индекс поля, по которому производится сортировка. -1 означает сортировку PivotField по меткам, остальные значения означают сортировку по полю данных.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotFieldSortSetting.SortBy. Этот метод будет удалён через 12 месяцев, начиная с сентября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


Указывает, будет ли применена простая операция сортировки данных.

**Remarks**

Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


Представляет индекс поля, по которому производится сортировка. Значение -1 указывает на сортировку по собственным значениям элемента сводки. При значении, большем или равном нулю, представляет индекс поля данных в области данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


Представляет [SortOrder](../../com.aspose.cells/sortorder).

См. [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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

