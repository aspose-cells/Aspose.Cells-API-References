---
title: "TextEffectFormat"
second_title: "Aspose.Cells for Java API 参考"
description: "包含适用于 WordArt 对象的属性和方法。"
type: docs
url: /zh/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

包含适用于 WordArt 对象的属性和方法。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
         TextEffectFormat textEffectFormat = shapes.get(0).getTextEffect();
         textEffectFormat.setTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10);
         workbook.save("Book1.xls");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | 指示字体是否为粗体。 |
| [getFontItalic()](#getFontItalic--) | 指示字体是否为斜体。 |
| [getFontName()](#getFontName--) | WordArt 中使用的字体名称。 |
| [getFontSize()](#getFontSize--) | WordArt 中使用的字体大小（以磅为单位）。 |
| [getPresetShape()](#getPresetShape--) | 获取预设形状类型。 |
| [getRotatedChars()](#getRotatedChars--) | 如果为 true，指定 WordArt 中的字符相对于 WordArt 的边界形状旋转 90 度。 |
| [getText()](#getText--) | WordArt 中的文本。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | 指示字体是否为粗体。 |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | 指示字体是否为斜体。 |
| [setFontName(String value)](#setFontName-java.lang.String-) | WordArt 中使用的字体名称。 |
| [setFontSize(int value)](#setFontSize-int-) | WordArt 中使用的字体大小（以磅为单位）。 |
| [setPresetShape(int value)](#setPresetShape-int-) | 设置预设形状类型。 |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | 如果为 true，指定 WordArt 中的字符相对于 WordArt 的边界形状旋转 90 度。 |
| [setText(String value)](#setText-java.lang.String-) | WordArt 中的文本。 |
| [setTextEffect(int effect)](#setTextEffect-int-) | 设置预设文本效果。 |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontBold() {#getFontBold--}
```
public boolean getFontBold()
```


指示字体是否为粗体。

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


指示字体是否为斜体。

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


WordArt 中使用的字体名称。

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


WordArt 中使用的字体大小（以磅为单位）。

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


获取预设形状类型。

参见 [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape)。

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


如果为 true，指定 WordArt 中的字符相对于 WordArt 的边界形状旋转 90 度。

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


WordArt 中的文本。

**Returns:**
java.lang.String
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




### setFontBold(boolean value) {#setFontBold-boolean-}
```
public void setFontBold(boolean value)
```


指示字体是否为粗体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


指示字体是否为斜体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


WordArt 中使用的字体名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


WordArt 中使用的字体大小（以磅为单位）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


设置预设形状类型。

参见 [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


如果为 true，指定 WordArt 中的字符相对于 WordArt 的边界形状旋转 90 度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


WordArt 中的文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


设置预设文本效果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect)。预设文本效果。 |

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

