---
title: "PivotItem"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет элемент в отчете PivotField."
type: docs
url: /ru/java/com.aspose.cells/pivotitem/
---

**Inheritance:**
java.lang.Object
```
public class PivotItem
```

Представляет элемент в отчете PivotField.

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
 
         //Hide the first item
         PivotItem item = rowField.getPivotItems().get(0);          
         item.setHidden(true);
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## Поля

| Поле | Описание |
| --- | --- |
| [ALL_PAGE_ITEMS_INDEX](#ALL-PAGE-ITEMS-INDEX) | Индекс‑сторож выбора всех элементов страницы (0x7FFD, недействительный индекс) |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDateTimeValue()](#getDateTimeValue--) | Получает значение даты и времени элемента сводки. Если значение равно null, будет возвращено DateTime.MinValue. |
| [getDoubleValue()](#getDoubleValue--) | Получает числовое значение типа double элемента сводки. Если значение равно null или не является числом, будет возвращено 0. |
| [getFormula()](#getFormula--) | Получает формулу этого вычисляемого элемента. |
| [getIndex()](#getIndex--) | Получает индекс элемента сводки в поле кэша. |
| [getName()](#getName--) | Получает имя элемента сводки. |
| [getPosition()](#getPosition--) | Указание индекса этого элемента во всех PivotItems поля. |
| [getPositionInSameParentNode()](#getPositionInSameParentNode--) | Указание индекса позиции в PivotItems под тем же родительским узлом. |
| [getStringValue()](#getStringValue--) | Получает строковое значение элемента сводки. Если значение равно null, будет возвращено "" |
| [getValue()](#getValue--) | Получает значение элемента сводки |
| [hashCode()](#hashCode--) |  |
| [hide(boolean value)](#hide-boolean-) | Устанавливает, скрыт ли элемент сводки. |
| [isCalculatedItem()](#isCalculatedItem--) | Указывает, является ли этот элемент сводки вычисляемым элементом формулы. |
| [isDetailHidden()](#isDetailHidden--) | Получает, скрыты ли детали этого элемента сводки. |
| [isFormula()](#isFormula--) | Указывает, является ли этот элемент сводки вычисляемым элементом формулы. |
| [isHidden()](#isHidden--) | Получает, скрыт ли элемент сводки. |
| [isHideDetail()](#isHideDetail--) | Получает, скрывает ли элемент сводки детали. |
| [isMissing()](#isMissing--) | Указывает, был ли элемент удалён из источника данных. |
| [move(int offset)](#move-int-) | Перемещает элемент вверх или вниз в поле сводки |
| [move(int offset, boolean isSameParent)](#move-int-boolean-) | Перемещает элемент вверх или вниз |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDetailHidden(boolean value)](#setDetailHidden-boolean-) | Устанавливает, скрыты ли детали этого элемента сводки. |
| [setFormula(boolean value)](#setFormula-boolean-) | Указывает, является ли этот элемент сводки вычисляемым элементом формулы. |
| [setHidden(boolean value)](#setHidden-boolean-) | Устанавливает, скрыт ли элемент сводки. |
| [setHideDetail(boolean value)](#setHideDetail-boolean-) | Устанавливает, скрывает ли элемент сводки детали. |
| [setIndex(int value)](#setIndex-int-) | Получает индекс элемента сводки в поле кэша. |
| [setName(String value)](#setName-java.lang.String-) | Получает имя элемента сводки. |
| [setPosition(int value)](#setPosition-int-) | Указание индекса этого элемента во всех PivotItems поля. |
| [setPositionInSameParentNode(int value)](#setPositionInSameParentNode-int-) | Указание индекса позиции в PivotItems под тем же родительским узлом. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALL_PAGE_ITEMS_INDEX {#ALL-PAGE-ITEMS-INDEX}
```
public static final short ALL_PAGE_ITEMS_INDEX
```


Индекс‑сторож выбора всех элементов страницы (0x7FFD, недействительный индекс)

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
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Получает значение даты и времени элемента сводки. Если значение равно null, будет возвращено DateTime.MinValue.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Получает числовое значение типа double элемента сводки. Если значение равно null или не является числом, будет возвращено 0.

**Returns:**
double
### getFormula() {#getFormula--}
```
public String getFormula()
```


Получает формулу этого вычисляемого элемента. Работает только когда элемент является вычисляемым.

**Returns:**
java.lang.String -
### getIndex() {#getIndex--}
```
public int getIndex()
```


Получает индекс элемента сводки в поле кэша.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotItem.Position. Этот метод будет удалён через 6 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Получает имя элемента сводки.

**Returns:**
java.lang.String
### getPosition() {#getPosition--}
```
public int getPosition()
```


Указание индекса этого элемента во всех PivotItems поля.

**Returns:**
int
### getPositionInSameParentNode() {#getPositionInSameParentNode--}
```
public int getPositionInSameParentNode()
```


Указание индекса позиции в PivotItems под тем же родительским узлом.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод PivotTable.MoveItem(PivotFieldType, string[],bool,int). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Получает строковое значение элемента сводки. Если значение равно null, будет возвращено ""

**Returns:**
java.lang.String
### getValue() {#getValue--}
```
public Object getValue()
```


Получает значение элемента сводки

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hide(boolean value) {#hide-boolean-}
```
public void hide(boolean value)
```


Устанавливает, скрыт ли элемент сводки.

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство Aspose.Cells.Pivot.PivotItem.IsHidden. Это свойство будет удалено через 12 месяцев, начиная с ЯНВАРЯ 2012 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### isCalculatedItem() {#isCalculatedItem--}
```
public boolean isCalculatedItem()
```


Указывает, является ли этот элемент сводки вычисляемым элементом формулы.

**Returns:**
boolean
### isDetailHidden() {#isDetailHidden--}
```
public boolean isDetailHidden()
```


Получает, скрыты ли детали этого элемента сводки.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Указывает, является ли этот элемент сводки вычисляемым элементом формулы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotItem.IsCalculatedItem. Это свойство будет удалено через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Получает, скрыт ли элемент сводки.

**Returns:**
boolean
### isHideDetail() {#isHideDetail--}
```
public boolean isHideDetail()
```


Получает, скрывает ли элемент сводки детали.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotItem.IsDetailHidden. Это свойство будет удалено через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
boolean
### isMissing() {#isMissing--}
```
public boolean isMissing()
```


Указывает, был ли элемент удалён из источника данных.

**Remarks**

True означает, что это значение было удалено из источника данных.

**Returns:**
boolean
### move(int offset) {#move-int-}
```
public void move(int offset)
```


Перемещает элемент вверх или вниз в поле сводки

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| смещение | int | Количество перемещений вверх или вниз. Переместите элемент вверх, если значение меньше нуля; переместите элемент вниз, если значение больше нуля. |

### move(int offset, boolean isSameParent) {#move-int-boolean-}
```
public void move(int offset, boolean isSameParent)
```


Перемещает элемент вверх или вниз

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод PivotTable.MoveItem(PivotFieldType, string[],bool,int) или метод PivotItem.Move(int). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| смещение | int | Количество перемещений вверх или вниз. Переместите элемент вверх, если значение меньше нуля; переместите элемент вниз, если значение больше нуля. |
| isSameParent | boolean | Указание, выполняется ли операция перемещения в том же родительском узле или нет |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDetailHidden(boolean value) {#setDetailHidden-boolean-}
```
public void setDetailHidden(boolean value)
```


Устанавливает, скрыты ли детали этого элемента сводки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setFormula(boolean value) {#setFormula-boolean-}
```
public void setFormula(boolean value)
```


Указывает, является ли этот элемент сводки вычисляемым элементом формулы.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotItem.IsCalculatedItem. Это свойство будет удалено через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Устанавливает, скрыт ли элемент сводки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setHideDetail(boolean value) {#setHideDetail-boolean-}
```
public void setHideDetail(boolean value)
```


Устанавливает, скрывает ли элемент сводки детали.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotItem.IsDetailHidden. Это свойство будет удалено через 12 месяцев, начиная с ноября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setIndex(int value) {#setIndex-int-}
```
public void setIndex(int value)
```


Получает индекс элемента сводки в поле кэша.

**Remarks**

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotItem.Position. Этот метод будет удалён через 6 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Получает имя элемента сводки.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Указание индекса этого элемента во всех PivotItems поля.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setPositionInSameParentNode(int value) {#setPositionInSameParentNode-int-}
```
public void setPositionInSameParentNode(int value)
```


Указание индекса позиции в PivotItems под тем же родительским узлом.

**Remarks**

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него используйте метод PivotTable.MoveItem(PivotFieldType, string[],bool,int). Этот метод будет удалён через 12 месяцев, начиная с ноября 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

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

