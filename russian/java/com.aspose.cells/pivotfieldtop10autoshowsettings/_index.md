---
title: "PivotFieldTop10AutoShowSettings"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет настройки AutoShow Top 10 для сводного поля."
type: docs
url: /ru/java/com.aspose.cells/pivotfieldtop10autoshowsettings/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldTop10AutoShowSettings
```

Представляет настройки AutoShow Top 10 для сводного поля.

**Remarks**

В xls: Реализация фильтров Top 10 в Xls через Top 10 AutoShow. В файлах ooxml: базовый формат ooxml поддерживает Top10 AutoShow, но пользовательский интерфейс Excel 2007 и более новых версий предоставляет доступ только через фильтр Top10. Если совместимость с XLS не требуется, рекомендуется использовать фильтр Top10 вместо этого.

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
 
         //Show top 2 items by row field label.
         rowField.top10AutoShow(true, true, 2, -1);
 
         PivotFieldTop10AutoShowSettings sortSetting = rowField.getTop10AutoShowSettings();
         System.out.println(sortSetting.isAutoShow());
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoShowCount()](#getAutoShowCount--) | Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы. |
| [getClass()](#getClass--) |  |
| [getRankBy()](#getRankBy--) | Указывает индекс поля данных для ранжирования AutoShow. |
| [hashCode()](#hashCode--) |  |
| [isAutoShow()](#isAutoShow--) | Указывает, применяется ли к этому полю фильтр "Top 10 AutoShow". |
| [isTop()](#isTop--) | Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoShow(boolean value)](#setAutoShow-boolean-) | Указывает, применяется ли к этому полю фильтр "Top 10 AutoShow". |
| [setAutoShowCount(int value)](#setAutoShowCount-int-) | Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы. |
| [setRankBy(int value)](#setRankBy-int-) | Указывает индекс поля данных для ранжирования AutoShow. |
| [setTop(boolean value)](#setTop-boolean-) | Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию. |
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
### getAutoShowCount() {#getAutoShowCount--}
```
public int getAutoShowCount()
```


Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRankBy() {#getRankBy--}
```
public int getRankBy()
```


Указывает индекс поля данных для ранжирования AutoShow. Представляет индекс поля автоотображения. -1 означает само поле PivotField. Должен быть индекс полей данных.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoShow() {#isAutoShow--}
```
public boolean isAutoShow()
```


Указывает, применяется ли к этому полю фильтр "Top 10 AutoShow".

**Returns:**
boolean
### isTop() {#isTop--}
```
public boolean isTop()
```


Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию.

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




### setAutoShow(boolean value) {#setAutoShow-boolean-}
```
public void setAutoShow(boolean value)
```


Указывает, применяется ли к этому полю фильтр "Top 10 AutoShow".

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setAutoShowCount(int value) {#setAutoShowCount-int-}
```
public void setAutoShowCount(int value)
```


Представляет количество верхних или нижних элементов, которые автоматически отображаются в указанном поле сводной таблицы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setRankBy(int value) {#setRankBy-int-}
```
public void setRankBy(int value)
```


Указывает индекс поля данных для ранжирования AutoShow. Представляет индекс поля автоотображения. -1 означает само поле PivotField. Должен быть индекс полей данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setTop(boolean value) {#setTop-boolean-}
```
public void setTop(boolean value)
```


Указывает, отображается ли указанное поле сводной таблицы автоматически по возрастанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

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

