---
title: "PivotShowValuesSetting"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройки отображения значений, когда используется вычисление ShowDataAs."
type: docs
url: /ru/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

Представляет настройки отображения значений, когда используется вычисление ShowDataAs.

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
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Поля

| Поле | Описание |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | Особый индекс базового элемента: использовать следующий элемент сводной таблицы. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | Особый индекс базового элемента: использовать предыдущий элемент сводной таблицы. |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | Представляет базовое поле для расчёта ShowDataAs, когда расчёт ShowDataAs используется. |
| [getBaseFieldName()](#getBaseFieldName--) | Получает подпись базового поля сводной таблицы. |
| [getBaseItemCaption()](#getBaseItemCaption--) | Получает подпись элемента сводной таблицы в базовом поле. |
| [getBaseItemIndex()](#getBaseItemIndex--) | Представляет пользовательский индекс элемента сводной таблицы в базовом поле, когда расчёт ShowDataAs используется. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | Представляет тип базового элемента сводной таблицы в базовом поле, когда используется вычисление ShowDataAs. |
| [getCalculationType()](#getCalculationType--) | Представляет способ отображения значений поля данных в сводном отчете. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | Получает способ отображения значений поля данных в сводном отчете. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | Представляет базовое поле для расчёта ShowDataAs, когда расчёт ShowDataAs используется. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | Представляет пользовательский индекс элемента сводной таблицы в базовом поле, когда расчёт ShowDataAs используется. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | Представляет тип базового элемента сводной таблицы в базовом поле, когда используется вычисление ShowDataAs. |
| [setCalculationType(int value)](#setCalculationType-int-) | Представляет способ отображения значений поля данных в сводном отчете. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | Устанавливает способ отображения значений поля данных в сводном отчете. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


Особый индекс базового элемента: использовать последующий элемент сводной таблицы. Действительно для вычислений "Show Values As"; применяется в Excel 2010 и более новых версиях.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


Особый индекс базового элемента: использовать предшествующий элемент сводной таблицы. Действительно для вычислений "Show Values As"; применяется в Excel 2010 и более новых версиях.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


Представляет базовое поле для расчёта ShowDataAs, когда расчёт ShowDataAs используется.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


Получает подпись базового поля сводной таблицы.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


Получает подпись элемента сводной таблицы в базовом поле.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


Представляет пользовательский индекс элемента сводной таблицы в базовом поле, когда расчёт ShowDataAs используется.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


Представляет тип базового элемента сводной таблицы в базовом поле, когда используется вычисление ShowDataAs. Поскольку PivotItemPosition.Custom доступен только для чтения, если необходимо установить PivotItemPosition.Custom, пожалуйста, задайте атрибут PivotField.BaseItemIndex.

Смотрите [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotShowValuesSetting.BaseItem. Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


Представляет способ отображения значений поля данных в сводном отчете.

Смотрите [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotShowValuesSetting.ShowValuesAs. Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


Получает способ отображения значений поля данных в сводном отчете.

Смотрите [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


Представляет базовое поле для расчёта ShowDataAs, когда расчёт ShowDataAs используется.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


Представляет пользовательский индекс элемента сводной таблицы в базовом поле, когда расчёт ShowDataAs используется.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


Представляет тип базового элемента сводной таблицы в базовом поле, когда используется вычисление ShowDataAs. Поскольку PivotItemPosition.Custom доступен только для чтения, если необходимо установить PivotItemPosition.Custom, пожалуйста, задайте атрибут PivotField.BaseItemIndex.

Смотрите [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotShowValuesSetting.BaseItem. Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


Представляет способ отображения значений поля данных в сводном отчете.

Смотрите [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте свойство PivotShowValuesSetting.ShowValuesAs. Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые причинённые неудобства.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


Устанавливает способ отображения значений поля данных в сводном отчете.

Смотрите [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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

