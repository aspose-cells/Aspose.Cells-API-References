---
title: "DataBar"
second_title: "Справочник API Aspose.Cells for Java"
description: "Описывает правило условного форматирования DataBar."
type: docs
url: /ru/java/com.aspose.cells/databar/
---

**Inheritance:**
java.lang.Object
```
public class DataBar
```

Опишите правило условного форматирования DataBar. Это правило условного форматирования отображает градиентную полоску данных в диапазоне ячеек.

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
         int idx = fcs.addCondition(FormatConditionType.DATA_BAR);
 
         fcs.addArea(ca);
 
         FormatCondition cond = fcs.get(idx);
 
         //Get Databar
         DataBar dataBar = cond.getDataBar();
 
         dataBar.setColor(Color.getOrange());
 
         //Set Databar properties
         dataBar.getMinCfvo().setType(FormatConditionValueType.PERCENTILE);
 
         dataBar.getMinCfvo().setValue(30);
 
         dataBar.setShowValue(false);
 
         dataBar.getBarBorder().setType(DataBarBorderType.SOLID);
 
         dataBar.getBarBorder().setColor(Color.getPlum());
 
          dataBar.setBarFillType(DataBarFillType.SOLID);
 
          dataBar.setAxisColor(Color.getRed());
 
          dataBar.setAxisPosition(DataBarAxisPosition.MIDPOINT);
 
          dataBar.getNegativeBarFormat().setColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setColor(Color.getWhite());
 
          dataBar.getNegativeBarFormat().setBorderColorType(DataBarNegativeColorType.COLOR);
 
          dataBar.getNegativeBarFormat().setBorderColor(Color.getYellow());
 
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
| [getAxisColor()](#getAxisColor--) | Получает цвет оси для ячеек с условным форматированием в виде полосок данных. |
| [getAxisPosition()](#getAxisPosition--) | Получает положение оси полосок данных, указанное правилом условного форматирования. |
| [getBarBorder()](#getBarBorder--) | Получает объект, задающий границу полоски данных. |
| [getBarFillType()](#getBarFillType--) | Получает способ заполнения полоски данных цветом. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Получает цвет этой DataBar. |
| [getDirection()](#getDirection--) | Получает направление отображения полоски данных. |
| [getMaxCfvo()](#getMaxCfvo--) | Получает объект максимального значения этой DataBar. |
| [getMaxLength()](#getMaxLength--) | Представляет максимальную длину полоски данных. |
| [getMinCfvo()](#getMinCfvo--) | Получает объект минимального значения этой DataBar. |
| [getMinLength()](#getMinLength--) | Представляет минимальную длину полоски данных. |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Получает объект NegativeBarFormat, связанный с правилом условного форматирования полоски данных. |
| [getShowValue()](#getShowValue--) | Получает флаг, указывающий, показывать ли значения ячеек, к которым применена эта полоска данных. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Получает цвет оси для ячеек с условным форматированием в виде полосок данных. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Устанавливает положение оси полосок данных, указанное правилом условного форматирования. |
| [setBarFillType(int value)](#setBarFillType-int-) | Устанавливает способ заполнения полоски данных цветом. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Устанавливает цвет этой DataBar. |
| [setDirection(int value)](#setDirection-int-) | Устанавливает направление отображения полоски данных. |
| [setMaxLength(int value)](#setMaxLength-int-) | Представляет максимальную длину полоски данных. |
| [setMinLength(int value)](#setMinLength-int-) | Представляет минимальную длину полоски данных. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Устанавливает флаг, указывающий, показывать ли значения ячеек, к которым применена эта полоска данных. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Отрисовывает полоску данных в ячейке в массив байтов изображения. |
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
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```


Получает цвет оси для ячеек с условным форматированием в виде полосок данных.

**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```


Получает положение оси полосок данных, указанное правилом условного форматирования.

См. [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```


Получает объект, задающий границу полоски данных.

**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```


Получает способ заполнения полоски данных цветом.

См. [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Получает цвет этой DataBar.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```


Получает направление отображения полоски данных.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```


Получает объект максимального значения этой DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Min.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```


Представляет максимальную длину полоски данных.

**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```


Получает объект минимального значения этой DataBar. Нельзя установить null или CFValueObject с типом FormatConditionValueType.Max.

**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```


Представляет минимальную длину полоски данных.

**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```


Получает объект NegativeBarFormat, связанный с правилом условного форматирования полоски данных.

**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Получает флаг, указывающий, показывать ли значения ячеек, к которым применена эта полоска данных. Значение по умолчанию — true.

**Returns:**
boolean
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




### setAxisColor(Color value) {#setAxisColor-com.aspose.cells.Color-}
```
public void setAxisColor(Color value)
```


Получает цвет оси для ячеек с условным форматированием в виде полосок данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```


Устанавливает положение оси полосок данных, указанное правилом условного форматирования.

См. [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```


Устанавливает способ заполнения полоски данных цветом.

См. [DataBarFillType](../../com.aspose.cells/databarfilltype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Устанавливает цвет этой DataBar.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```


Устанавливает направление отображения полоски данных.

См. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```


Представляет максимальную длину полоски данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```


Представляет минимальную длину полоски данных.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Устанавливает флаг, указывающий, следует ли показывать значения ячеек, к которым применяется эта полоска данных. Значение по умолчанию — true.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```


Отрисовывает полоску данных в ячейке в массив байтов изображения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Указывает, в какой ячейке должна отображаться полоска данных |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions содержит некоторые свойства выходного изображения |

**Returns:**
byte[] -
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

