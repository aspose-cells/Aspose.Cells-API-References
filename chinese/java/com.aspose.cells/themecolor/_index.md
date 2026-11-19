---
title: "ThemeColor"
second_title: "Aspose.Cells for Java API 参考"
description: "表示主题颜色。"
type: docs
url: /zh/java/com.aspose.cells/themecolor/
---

**Inheritance:**
java.lang.Object
```
public class ThemeColor
```

表示主题颜色。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Hello World");
         Style style = cells.get("A1").getStyle();
         //Set ThemeColorType.Text2 color type with 40% lighten as the font color.
         style.getFont().setThemeColor(new ThemeColor(ThemeColorType.TEXT_2, 0.4));
         style.setPattern(BackgroundType.SOLID);
         //Set ThemeColorType.Background2 color type with 75% darken as the foreground color
         style.setForegroundThemeColor(new ThemeColor(ThemeColorType.BACKGROUND_2, -0.75));
         cells.get("A1").setStyle(style);
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ThemeColor(int type, double tint)](#ThemeColor-int-double-) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorType()](#getColorType--) | 获取主题类型。 |
| [getTint()](#getTint--) | 获取色调值。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColorType(int value)](#setColorType-int-) | 设置主题类型。 |
| [setTint(double value)](#setTint-double-) | 设置色调值。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ThemeColor(int type, double tint) {#ThemeColor-int-double-}
```
public ThemeColor(int type, double tint)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype)。主题类型。 |
| tint | double | 色调值。 |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorType() {#getColorType--}
```
public int getColorType()
```


获取主题类型。

参见 [ThemeColorType](../../com.aspose.cells/themecolortype)。

**Returns:**
int
### getTint() {#getTint--}
```
public double getTint()
```


获取色调值。

**Remarks**

色调值以 double 类型存储，范围为 -1.0 到 1.0，其中 -1.0 表示 100% 加暗，1.0 表示 100% 加亮。另外，0.0 表示无变化。

**Returns:**
double
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




### setColorType(int value) {#setColorType-int-}
```
public void setColorType(int value)
```


设置主题类型。

参见 [ThemeColorType](../../com.aspose.cells/themecolortype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTint(double value) {#setTint-double-}
```
public void setTint(double value)
```


设置色调值。

**Remarks**

色调值以 double 类型存储，范围为 -1.0 到 1.0，其中 -1.0 表示 100% 加暗，1.0 表示 100% 加亮。另外，0.0 表示无变化。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

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

