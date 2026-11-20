---
title: "Top10"
second_title: "Справочник API Aspose.Cells for Java"
description: "Описание правила условного форматирования Top10."
type: docs
url: /ru/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

Опишите правило условного форматирования Top10. Это правило условного форматирования выделяет ячейки, значения которых находятся в верхних N или нижних N диапазонах, как указано.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = CellArea.createCellArea(0, 0, 10, 10);
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.TOP_10, OperatorType.NONE, null, null);   
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         Top10 top10 = fc.getTop10();
         //Set the Top N 
         top10.setRank(5);  
         //Saving the Excel file
         workbook.save("output.xls");
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Top10()](#Top10--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Получает значение "n" в правиле условного форматирования "top/bottom n". |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Получает, является ли правило "top/bottom n" правилом "bottom n". |
| [isPercent()](#isPercent--) | Получает, является ли правило "top/bottom n" правилом "top/bottom n percent". |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Устанавливает, является ли правило "top/bottom n" правилом "bottom n". |
| [setPercent(boolean value)](#setPercent-boolean-) | Устанавливает, является ли правило "top/bottom n" правилом "top/bottom n percent". |
| [setRank(int value)](#setRank-int-) | Устанавливает значение "n" в правиле условного форматирования "top/bottom n". |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Top10() {#Top10--}
```
public Top10()
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
### getRank() {#getRank--}
```
public int getRank()
```


Получает значение "n" в правиле условного форматирования "top/bottom n". Если IsPercent равно true, значение должно быть от 0 до 100. В противном случае оно должно быть от 0 до 1000. Значение по умолчанию — 10.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Получает, является ли правило "top/bottom n" правилом "bottom n". Значение по умолчанию — false.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Получает, является ли правило "top/bottom n" правилом "top/bottom n percent". Значение по умолчанию — false.

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




### setBottom(boolean value) {#setBottom-boolean-}
```
public void setBottom(boolean value)
```


Устанавливает, является ли правило "top/bottom n" правилом "bottom n". Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


Устанавливает, является ли правило "top/bottom n" правилом "top/bottom n percent". Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


Устанавливает значение "n" в правиле условного форматирования "top/bottom n". Если IsPercent равно true, значение должно быть от 0 до 100. В противном случае оно должно быть от 0 до 1000. Значение по умолчанию — 10.

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

