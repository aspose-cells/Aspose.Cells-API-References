---
title: "الحد"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل حد الخلية."
type: docs
url: /ar/java/com.aspose.cells/border/
---

**Inheritance:**
java.lang.Object
```
public class Border
```

يحتوي على الكائن الذي يمثل حد الخلية.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | يحصل على اللون بقيمة ARGB 32-بت. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يحصل على [Color](../../com.aspose.cells/color) للحد. |
| [getLineStyle()](#getLineStyle--) | يحصل على نوع حد الخلية. |
| [getThemeColor()](#getThemeColor--) | يحصل على لون السمة للحد. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | يضبط اللون بقيمة ARGB 32-بت. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يضبط [Color](../../com.aspose.cells/color) للحد. |
| [setLineStyle(int value)](#setLineStyle-int-) | يضبط نوع حد الخلية. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | يضبط لون السمة للحد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


يحصل على اللون بقيمة ARGB 32-بت.

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


يحصل على [Color](../../com.aspose.cells/color) للحد.

**Returns:**
[Color](../../com.aspose.cells/color)
### getLineStyle() {#getLineStyle--}
```
public int getLineStyle()
```


يحصل على نوع حد الخلية.

انظر [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


يحصل على لون السمة للحد.

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


يضبط اللون بقيمة ARGB 32-بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


يضبط [Color](../../com.aspose.cells/color) للحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setLineStyle(int value) {#setLineStyle-int-}
```
public void setLineStyle(int value)
```


يضبط نوع حد الخلية.

انظر [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


يضبط لون السمة للحد.

**Parameters:**
| معامل | نوع | الوصف |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

