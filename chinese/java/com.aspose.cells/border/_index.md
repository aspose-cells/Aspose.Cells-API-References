---
title: "Border"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示单元格边框的对象。"
type: docs
url: /zh/java/com.aspose.cells/border/
---

**Inheritance:**
java.lang.Object
```
public class Border
```

封装表示单元格边框的对象。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | 获取具有 32 位 ARGB 值的颜色。 |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | 获取边框的 [Color](../../com.aspose.cells/color)。 |
| [getLineStyle()](#getLineStyle--) | 获取单元格边框类型。 |
| [getThemeColor()](#getThemeColor--) | 获取边框的主题颜色。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | 使用 32 位 ARGB 值设置颜色。 |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | 设置边框的 [Color](../../com.aspose.cells/color)。 |
| [setLineStyle(int value)](#setLineStyle-int-) | 设置单元格边框类型。 |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | 设置边框的主题颜色。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


获取具有 32 位 ARGB 值的颜色。

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


获取边框的 [Color](../../com.aspose.cells/color)。

**Returns:**
[Color](../../com.aspose.cells/color)
### getLineStyle() {#getLineStyle--}
```
public int getLineStyle()
```


获取单元格边框类型。

参见 [CellBorderType](../../com.aspose.cells/cellbordertype)。

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


获取边框的主题颜色。

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


使用 32 位 ARGB 值设置颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


设置边框的 [Color](../../com.aspose.cells/color)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setLineStyle(int value) {#setLineStyle-int-}
```
public void setLineStyle(int value)
```


设置单元格边框类型。

参见 [CellBorderType](../../com.aspose.cells/cellbordertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


设置边框的主题颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

