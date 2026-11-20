---
title: "BorderCollection"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует коллекцию объектов."
type: docs
url: /ru/java/com.aspose.cells/bordercollection/
---

**Inheritance:**
java.lang.Object
```
public class BorderCollection
```

Инкапсулирует коллекцию объектов [Border](../../com.aspose.cells/border).

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Adding a new worksheet to the Excel object
         workbook.getWorksheets().add();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Visit Aspose!");
 
         Style style = cell.getStyle();
 
         //Setting the line style of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the top border
         style.getBorders().getByBorderType(BorderType.TOP_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the bottom border
         style.getBorders().getByBorderType(BorderType.BOTTOM_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the left border
         style.getBorders().getByBorderType(BorderType.LEFT_BORDER).setColor(Color.getBlack());
 
         //Setting the line style of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setLineStyle(CellBorderType.THICK);
 
         //Setting the color of the right border
         style.getBorders().getByBorderType(BorderType.RIGHT_BORDER).setColor(Color.getBlack());
 
         cell.setStyle(style);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getByBorderType(int borderType)](#getByBorderType-int-) | Получает элемент [Border](../../com.aspose.cells/border) по указанному индексу. |
| [getClass()](#getClass--) |  |
| [getDiagonalColor()](#getDiagonalColor--) | Получает [Color](../../com.aspose.cells/color) диагональных линий. |
| [getDiagonalStyle()](#getDiagonalStyle--) | Получает стиль диагональных линий. |
| [hashCode()](#hashCode--) |  |
| [isOutline()](#isOutline--) | Указывает, следует ли применять левую, правую, верхнюю и нижнюю границы только к внешним границам диапазона ячеек. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColor(Color color)](#setColor-com.aspose.cells.Color-) | Устанавливает [Color](../../com.aspose.cells/color) всех границ в коллекции. |
| [setDiagonalColor(Color value)](#setDiagonalColor-com.aspose.cells.Color-) | Устанавливает [Color](../../com.aspose.cells/color) диагональных линий. |
| [setDiagonalStyle(int value)](#setDiagonalStyle-int-) | Устанавливает стиль диагональных линий. |
| [setOutline(boolean value)](#setOutline-boolean-) | Указывает, следует ли применять левую, правую, верхнюю и нижнюю границы только к внешним границам диапазона ячеек. |
| [setStyle(int style)](#setStyle-int-) | Устанавливает стиль всех границ коллекции. |
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
### getByBorderType(int borderType) {#getByBorderType-int-}
```
public Border getByBorderType(int borderType)
```


Получает элемент [Border](../../com.aspose.cells/border) по указанному индексу.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Граница, которую необходимо получить. |

**Returns:**
[Border](../../com.aspose.cells/border) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDiagonalColor() {#getDiagonalColor--}
```
public Color getDiagonalColor()
```


Получает [Color](../../com.aspose.cells/color) диагональных линий.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDiagonalStyle() {#getDiagonalStyle--}
```
public int getDiagonalStyle()
```


Получает стиль диагональных линий.

См. [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


Указывает, следует ли применять левую, правую, верхнюю и нижнюю границы только к внешним границам диапазона ячеек. Значение по умолчанию — true.

**Remarks**

Работает только при применении к диапазону для условного форматирования, сводных таблиц. Если false, левая, правая, верхняя и нижняя границы будут применяться к каждой ячейке, иначе только к внешним границам диапазона ячеек. Если true, пожалуйста, установите горизонтальные и вертикальные границы внутренних границ диапазона для условного форматирования, сводных таблиц.

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




### setColor(Color color) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color color)
```


Устанавливает [Color](../../com.aspose.cells/color) всех границ в коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Цвет [Color](../../com.aspose.cells/color) границ. |

### setDiagonalColor(Color value) {#setDiagonalColor-com.aspose.cells.Color-}
```
public void setDiagonalColor(Color value)
```


Устанавливает [Color](../../com.aspose.cells/color) диагональных линий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDiagonalStyle(int value) {#setDiagonalStyle-int-}
```
public void setDiagonalStyle(int value)
```


Устанавливает стиль диагональных линий.

См. [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


Указывает, следует ли применять левую, правую, верхнюю и нижнюю границы только к внешним границам диапазона ячеек. Значение по умолчанию — true.

**Remarks**

Работает только при применении к диапазону для условного форматирования, сводных таблиц. Если false, левая, правая, верхняя и нижняя границы будут применяться к каждой ячейке, иначе только к внешним границам диапазона ячеек. Если true, пожалуйста, установите горизонтальные и вертикальные границы внутренних границ диапазона для условного форматирования, сводных таблиц.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setStyle(int style) {#setStyle-int-}
```
public void setStyle(int style)
```


Устанавливает стиль всех границ коллекции.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| style | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Стиль границ |

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

