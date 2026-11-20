---
title: "IconSet"
second_title: "Справочник API Aspose.Cells for Java"
description: "Описывает правило условного форматирования IconSet."
type: docs
url: /ru/java/com.aspose.cells/iconset/
---

**Inheritance:**
java.lang.Object
```
public class IconSet
```

Опишите правило условного форматирования IconSet. Это правило условного форматирования применяет значки к ячейкам в соответствии с их значениями.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
 
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
 
         ca.StartRow = 0;
 
         ca.EndRow = 2;
 
         ca.StartColumn = 0;
 
         ca.EndColumn = 0;
 
         fcs.addArea(ca);
 
         //Adds condition.
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Icon Set
         IconSet iconSet = cond.getIconSet();
 
         //Set Icon Type
         iconSet.setType(IconSetType.ARROWS_3);
 
         //Put Cell Values
         Cell cell1 = sheet.getCells().get("A1");
 
         cell1.putValue(10);
 
         Cell cell2 = sheet.getCells().get("A2");
 
         cell2.putValue(120);
 
         Cell cell3 = sheet.getCells().get("A3");
 
         cell3.putValue(260);
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCfIcons()](#getCfIcons--) | Получите [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) из коллекции |
| [getCfvos()](#getCfvos--) | Получите экземпляр CFValueObjects. |
| [getClass()](#getClass--) |  |
| [getReverse()](#getReverse--) | Возвращает флаг, указывающий, следует ли изменить порядок значков по умолчанию в этом наборе значков. |
| [getShowValue()](#getShowValue--) | Возвращает флаг, указывающий, следует ли показывать значения ячеек, к которым применяется этот набор значков. |
| [getType()](#getType--) | Возвращает тип набора значков для отображения. |
| [hashCode()](#hashCode--) |  |
| [isCustom()](#isCustom--) | Указывает, является ли набор значков пользовательским. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setReverse(boolean value)](#setReverse-boolean-) | Устанавливает флаг, указывающий, следует ли изменить порядок значков по умолчанию в этом наборе значков. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Устанавливает флаг, указывающий, следует ли показывать значения ячеек, к которым применяется этот набор значков. |
| [setType(int value)](#setType-int-) | Устанавливает тип набора значков для отображения. |
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
### getCfIcons() {#getCfIcons--}
```
public ConditionalFormattingIconCollection getCfIcons()
```


Получите [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) из коллекции

**Returns:**
[ConditionalFormattingIconCollection](../../com.aspose.cells/conditionalformattingiconcollection)
### getCfvos() {#getCfvos--}
```
public ConditionalFormattingValueCollection getCfvos()
```


Получите экземпляр CFValueObjects.

**Returns:**
[ConditionalFormattingValueCollection](../../com.aspose.cells/conditionalformattingvaluecollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getReverse() {#getReverse--}
```
public boolean getReverse()
```


Возвращает флаг, указывающий, следует ли изменить порядок значков по умолчанию в этом наборе значков. Значение по умолчанию — false.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Возвращает флаг, указывающий, следует ли показывать значения ячеек, к которым применяется этот набор значков. Значение по умолчанию — true.

**Returns:**
boolean
### getType() {#getType--}
```
public int getType()
```


Возвращает тип набора значков для отображения. Установка типа автоматически проверит, соответствует ли количество текущих Cfvos новому типу. Если не соответствует, старые Cfvos будут удалены, и будут добавлены значения Cfvos по умолчанию.

Смотрите [IconSetType](../../com.aspose.cells/iconsettype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCustom() {#isCustom--}
```
public boolean isCustom()
```


Указывает, является ли набор значков пользовательским. Значение по умолчанию — false.

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




### setReverse(boolean value) {#setReverse-boolean-}
```
public void setReverse(boolean value)
```


Устанавливает флаг, указывающий, следует ли изменить порядок значков по умолчанию в этом наборе значков. Значение по умолчанию — false.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Устанавливает флаг, указывающий, следует ли показывать значения ячеек, к которым применяется этот набор значков. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Устанавливает тип набора значков для отображения. При установке типа будет автоматически проверяться, соответствует ли количество текущих Cfvos новому типу. Если не соответствует, старые Cfvos будут удалены, а будут добавлены значения Cfvos по умолчанию.

Смотрите [IconSetType](../../com.aspose.cells/iconsettype).

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

