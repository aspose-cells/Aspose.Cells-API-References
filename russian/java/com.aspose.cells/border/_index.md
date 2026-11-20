---
title: "Граница"
second_title: "Справочник API Aspose.Cells for Java"
description: "Инкапсулирует объект, представляющий границу ячейки."
type: docs
url: /ru/java/com.aspose.cells/border/
---

**Inheritance:**
java.lang.Object
```
public class Border
```

Инкапсулирует объект, представляющий границу ячейки.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
 
         Style style = cell.getStyle();
         //Set top border style and color
         Border border = style.getBorders().getByBorderType(BorderType.TOP_BORDER);
         border.setLineStyle(CellBorderType.MEDIUM);
         border.setColor(Color.getRed());
         cell.setStyle(style);
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Получает цвет в виде 32-битного значения ARGB. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Получает [Color](../../com.aspose.cells/color) границы. |
| [getLineStyle()](#getLineStyle--) | Получает тип границы ячейки. |
| [getThemeColor()](#getThemeColor--) | Получает цвет темы границы. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Устанавливает цвет в виде 32-битного значения ARGB. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Устанавливает [Color](../../com.aspose.cells/color) границы. |
| [setLineStyle(int value)](#setLineStyle-int-) | Устанавливает тип границы ячейки. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Устанавливает цвет темы границы. |
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Получает цвет в виде 32-битного значения ARGB.

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


Получает [Color](../../com.aspose.cells/color) границы.

**Returns:**
[Color](../../com.aspose.cells/color)
### getLineStyle() {#getLineStyle--}
```
public int getLineStyle()
```


Получает тип границы ячейки.

См. [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Получает цвет темы границы.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Устанавливает цвет в виде 32-битного значения ARGB.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Устанавливает [Color](../../com.aspose.cells/color) границы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setLineStyle(int value) {#setLineStyle-int-}
```
public void setLineStyle(int value)
```


Устанавливает тип границы ячейки.

См. [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Устанавливает цвет темы границы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

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

