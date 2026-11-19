---
title: "ImageActiveXControl"
second_title: "Aspose.Cells for Java API 参考"
description: "表示图像控件。"
type: docs
url: /zh/java/com.aspose.cells/imageactivexcontrol/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ActiveXControlBase](../../com.aspose.cells/activexcontrolbase), [com.aspose.cells.ActiveXControl](../../com.aspose.cells/activexcontrol)
```
public class ImageActiveXControl extends ActiveXControl
```

表示图像控件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | 获取背景的 ole 颜色。 |
| [getBorderOleColor()](#getBorderOleColor--) | 获取背景的 ole 颜色。 |
| [getBorderStyle()](#getBorderStyle--) | 获取控件使用的边框类型。 |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | 获取控件的二进制数据。 |
| [getFont()](#getFont--) | 表示控件的字体。 |
| [getForeOleColor()](#getForeOleColor--) | 获取前景的 OLE 颜色。 |
| [getHeight()](#getHeight--) | 获取控件的高度（单位为点）。 |
| [getIMEMode()](#getIMEMode--) | 获取控件获得焦点时输入法编辑器的默认运行模式。 |
| [getLinkedCell()](#getLinkedCell--) | 获取链接的单元格。 |
| [getListFillRange()](#getListFillRange--) | 获取列表填充范围。 |
| [getMouseIcon()](#getMouseIcon--) | 获取用于在控件上显示为鼠标指针的自定义图标。 |
| [getMousePointer()](#getMousePointer--) | 获取在控件上显示为鼠标指针的图标类型。 |
| [getPicture()](#getPicture--) | 获取图片的数据。 |
| [getPictureAlignment()](#getPictureAlignment--) | 获取 Form 或 Image 中图片的对齐方式。 |
| [getPictureSizeMode()](#getPictureSizeMode--) | 获取图片的显示方式。 |
| [getShadow()](#getShadow--) | 指示是否显示阴影。 |
| [getSpecialEffect()](#getSpecialEffect--) | 获取控件的特殊效果。 |
| [getTextAlign()](#getTextAlign--) | 表示控件使用的文本对齐方式。 |
| [getType()](#getType--) | 获取 ActiveX 控件的类型。 |
| [getWidth()](#getWidth--) | 获取控件的宽度（单位为点）。 |
| [getWorkbook()](#getWorkbook--) | 获取 [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) 对象。 |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [isEnabled()](#isEnabled--) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [isLocked()](#isLocked--) | 指示控件中的数据是否被锁定，无法编辑。 |
| [isTiled()](#isTiled--) | 指示图片是否在背景上平铺。 |
| [isTransparent()](#isTransparent--) | 指示控件是否透明。 |
| [isVisible()](#isVisible--) | 指示此控件是否可见。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | 指示控件是否会自动调整大小以显示其全部内容。 |
| [setBackOleColor(int value)](#setBackOleColor-int-) | 设置背景的 OLE 颜色。 |
| [setBorderOleColor(int value)](#setBorderOleColor-int-) | 设置背景的 OLE 颜色。 |
| [setBorderStyle(int value)](#setBorderStyle-int-) | 设置控件使用的边框类型。 |
| [setEnabled(boolean value)](#setEnabled-boolean-) | 指示控件是否可以获取焦点并响应用户生成的事件。 |
| [setForeOleColor(int value)](#setForeOleColor-int-) | 设置前景的 OLE 颜色。 |
| [setHeight(double value)](#setHeight-double-) | 设置控件的高度（单位为点）。 |
| [setIMEMode(int value)](#setIMEMode-int-) | 设置控件获取焦点时输入法编辑器的默认运行模式。 |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | 设置链接的单元格。 |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | 设置列表填充范围。 |
| [setLocked(boolean value)](#setLocked-boolean-) | 指示控件中的数据是否被锁定，无法编辑。 |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | 设置自定义图标，以在控件上显示为鼠标指针。 |
| [setMousePointer(int value)](#setMousePointer-int-) | 设置在控件上显示为鼠标指针的图标类型。 |
| [setPicture(byte[] value)](#setPicture-byte---) | 设置图片的数据。 |
| [setPictureAlignment(int value)](#setPictureAlignment-int-) | 设置 Form 或 Image 中图片的对齐方式。 |
| [setPictureSizeMode(int value)](#setPictureSizeMode-int-) | 设置图片的显示方式。 |
| [setShadow(boolean value)](#setShadow-boolean-) | 指示是否显示阴影。 |
| [setSpecialEffect(int value)](#setSpecialEffect-int-) | 设置控件的特殊效果。 |
| [setTextAlign(int value)](#setTextAlign-int-) | 表示控件使用的文本对齐方式。 |
| [setTiled(boolean value)](#setTiled-boolean-) | 指示图片是否在背景上平铺。 |
| [setTransparent(boolean value)](#setTransparent-boolean-) | 指示控件是否透明。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示此控件是否可见。 |
| [setWidth(double value)](#setWidth-double-) | 以点为单位设置控件的宽度。 |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


获取背景的 ole 颜色。

**Returns:**
int
### getBorderOleColor() {#getBorderOleColor--}
```
public int getBorderOleColor()
```


获取背景的 ole 颜色。

**Returns:**
int
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


获取控件使用的边框类型。

参见 [ControlBorderType](../../com.aspose.cells/controlbordertype)。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


获取控件的二进制数据。

**Returns:**
byte[]
### getFont() {#getFont--}
```
public Font getFont()
```


表示控件的字体。

**Returns:**
[Font](../../com.aspose.cells/font)
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


获取前景的 OLE 颜色。

**Remarks**

不适用于 Image 控件。

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


获取控件的高度（单位为点）。

**Returns:**
double
### getIMEMode() {#getIMEMode--}
```
public int getIMEMode()
```


获取控件获得焦点时输入法编辑器的默认运行模式。

参见 [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode)。

**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


获取链接的单元格。

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


获取列表填充范围。

**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


获取用于在控件上显示为鼠标指针的自定义图标。

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


获取在控件上显示为鼠标指针的图标类型。

参见 [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype)。

**Returns:**
int
### getPicture() {#getPicture--}
```
public byte[] getPicture()
```


获取图片的数据。

**Returns:**
byte[]
### getPictureAlignment() {#getPictureAlignment--}
```
public int getPictureAlignment()
```


获取 Form 或 Image 中图片的对齐方式。

参见 [ControlPictureAlignmentType](../../com.aspose.cells/controlpicturealignmenttype)。

**Returns:**
int
### getPictureSizeMode() {#getPictureSizeMode--}
```
public int getPictureSizeMode()
```


获取图片的显示方式。

参见 [ControlPictureSizeMode](../../com.aspose.cells/controlpicturesizemode)。

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


指示是否显示阴影。

**Returns:**
boolean
### getSpecialEffect() {#getSpecialEffect--}
```
public int getSpecialEffect()
```


获取控件的特殊效果。

参见 [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype)。

**Returns:**
int
### getTextAlign() {#getTextAlign--}
```
public int getTextAlign()
```


表示控件使用的文本对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


获取 ActiveX 控件的类型。

参见 [ControlType](../../com.aspose.cells/controltype)。

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


获取控件的宽度（单位为点）。

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


获取 [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) 对象。

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


指示控件是否会自动调整大小以显示其全部内容。

**Returns:**
boolean
### isEnabled() {#isEnabled--}
```
public boolean isEnabled()
```


指示控件是否可以获取焦点并响应用户生成的事件。

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


指示控件中的数据是否被锁定，无法编辑。

**Returns:**
boolean
### isTiled() {#isTiled--}
```
public boolean isTiled()
```


指示图片是否在背景上平铺。

**Returns:**
boolean
### isTransparent() {#isTransparent--}
```
public boolean isTransparent()
```


指示控件是否透明。

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


指示此控件是否可见。

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




### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


指示控件是否会自动调整大小以显示其全部内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


设置背景的 OLE 颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBorderOleColor(int value) {#setBorderOleColor-int-}
```
public void setBorderOleColor(int value)
```


设置背景的 OLE 颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


设置控件使用的边框类型。

参见 [ControlBorderType](../../com.aspose.cells/controlbordertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


指示控件是否可以获取焦点并响应用户生成的事件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


设置前景的 OLE 颜色。

**Remarks**

不适用于 Image 控件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


设置控件的高度（单位为点）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setIMEMode(int value) {#setIMEMode-int-}
```
public void setIMEMode(int value)
```


设置控件获取焦点时输入法编辑器的默认运行模式。

参见 [InputMethodEditorMode](../../com.aspose.cells/inputmethodeditormode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


设置链接的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


设置列表填充范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


指示控件中的数据是否被锁定，无法编辑。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


设置自定义图标，以在控件上显示为鼠标指针。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


设置在控件上显示为鼠标指针的图标类型。

参见 [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPicture(byte[] value) {#setPicture-byte---}
```
public void setPicture(byte[] value)
```


设置图片的数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setPictureAlignment(int value) {#setPictureAlignment-int-}
```
public void setPictureAlignment(int value)
```


设置 Form 或 Image 中图片的对齐方式。

参见 [ControlPictureAlignmentType](../../com.aspose.cells/controlpicturealignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPictureSizeMode(int value) {#setPictureSizeMode-int-}
```
public void setPictureSizeMode(int value)
```


设置图片的显示方式。

参见 [ControlPictureSizeMode](../../com.aspose.cells/controlpicturesizemode)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


指示是否显示阴影。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSpecialEffect(int value) {#setSpecialEffect-int-}
```
public void setSpecialEffect(int value)
```


设置控件的特殊效果。

参见 [ControlSpecialEffectType](../../com.aspose.cells/controlspecialeffecttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextAlign(int value) {#setTextAlign-int-}
```
public void setTextAlign(int value)
```


表示控件使用的文本对齐方式。

参见 [TextAlignmentType](../../com.aspose.cells/textalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTiled(boolean value) {#setTiled-boolean-}
```
public void setTiled(boolean value)
```


指示图片是否在背景上平铺。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


指示控件是否透明。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


指示此控件是否可见。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


以点为单位设置控件的宽度。

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

