---
title: Border
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents the cell border.
type: docs
weight: 40
url: /java/com.aspose.cells/border/
---

**Inheritance:**
java.lang.Object
```
public class Border
```

Encapsulates the object that represents the cell border.

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
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Gets and sets the color with a 32-bit ARGB value. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets or sets the [Color](../../com.aspose.cells/color) of the border. |
| [getLineStyle()](#getLineStyle--) | Gets or sets the cell border type. |
| [getThemeColor()](#getThemeColor--) | Gets and sets the theme color of the border. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | For the description of this property, please see \#getArgbColor().getArgbColor() |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | For the description of this property, please see \#getColor().getColor() |
| [setLineStyle(int value)](#setLineStyle-int-) | For the description of this property, please see \#getLineStyle().getLineStyle() |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | For the description of this property, please see \#getThemeColor().getThemeColor() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Gets and sets the color with a 32-bit ARGB value.

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


Gets or sets the [Color](../../com.aspose.cells/color) of the border.

**Returns:**
[Color](../../com.aspose.cells/color)
### getLineStyle() {#getLineStyle--}
```
public int getLineStyle()
```


Gets or sets the cell border type.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Gets and sets the theme color of the border.

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


For the description of this property, please see \#getArgbColor().getArgbColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


For the description of this property, please see \#getColor().getColor()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setLineStyle(int value) {#setLineStyle-int-}
```
public void setLineStyle(int value)
```


For the description of this property, please see \#getLineStyle().getLineStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


For the description of this property, please see \#getThemeColor().getThemeColor()

**Parameters:**
| Parameter | Type | Description |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

