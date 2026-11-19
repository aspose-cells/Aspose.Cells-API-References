---
title: "MsoFormatPicture"
second_title: "Aspose.Cells for Java API 参考"
description: "表示图片格式。"
type: docs
url: /zh/java/com.aspose.cells/msoformatpicture/
---

**Inheritance:**
java.lang.Object
```
public class MsoFormatPicture
```

表示图片格式。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomCrop()](#getBottomCrop--) | 表示裁剪矩形底部位置，以图像高度的比例表示。 |
| [getBottomCropInch()](#getBottomCropInch--) | 表示裁剪矩形底部位置，以英寸为单位表示。 |
| [getBrightness()](#getBrightness--) | 表示图片的亮度修改，以百分比为单位。 |
| [getClass()](#getClass--) |  |
| [getContrast()](#getContrast--) | 表示图片的对比度修改，以百分比为单位。 |
| [getGamma()](#getGamma--) | 表示图片的伽马值。 |
| [getLeftCrop()](#getLeftCrop--) | 表示裁剪矩形左侧位置，以图像宽度的比例表示。 |
| [getLeftCropInch()](#getLeftCropInch--) | 表示裁剪矩形左侧位置，以英寸为单位。 |
| [getRightCrop()](#getRightCrop--) | 表示裁剪矩形右侧位置，以图像宽度的比例表示。 |
| [getRightCropInch()](#getRightCropInch--) | 表示裁剪矩形右侧位置，以英寸为单位。 |
| [getTopCrop()](#getTopCrop--) | 表示裁剪矩形顶部位置，以图像高度的比例表示。 |
| [getTopCropInch()](#getTopCropInch--) | 表示裁剪矩形顶部位置，以英寸为单位。 |
| [getTransparency()](#getTransparency--) | 返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [getTransparentColor()](#getTransparentColor--) | 获取图片的透明颜色。 |
| [hashCode()](#hashCode--) | 获取哈希码。 |
| [isBiLevel()](#isBiLevel--) | 指示此图片是否应以双色黑白显示。 |
| [isGray()](#isGray--) | 指示此图片是否应以灰度显示。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBiLevel(boolean value)](#setBiLevel-boolean-) | 指示此图片是否应以双色黑白显示。 |
| [setBottomCrop(double value)](#setBottomCrop-double-) | 表示裁剪矩形底部位置，以图像高度的比例表示。 |
| [setBottomCropInch(double value)](#setBottomCropInch-double-) | 表示裁剪矩形底部位置，以英寸为单位表示。 |
| [setBrightness(double value)](#setBrightness-double-) | 表示图片的亮度修改，以百分比为单位。 |
| [setContrast(double value)](#setContrast-double-) | 表示图片的对比度修改，以百分比为单位。 |
| [setGamma(double value)](#setGamma-double-) | 表示图片的伽马值。 |
| [setGray(boolean value)](#setGray-boolean-) | 指示此图片是否应以灰度显示。 |
| [setLeftCrop(double value)](#setLeftCrop-double-) | 表示裁剪矩形左侧位置，以图像宽度的比例表示。 |
| [setLeftCropInch(double value)](#setLeftCropInch-double-) | 表示裁剪矩形左侧位置，以英寸为单位。 |
| [setRightCrop(double value)](#setRightCrop-double-) | 表示裁剪矩形右侧位置，以图像宽度的比例表示。 |
| [setRightCropInch(double value)](#setRightCropInch-double-) | 表示裁剪矩形右侧位置，以英寸为单位。 |
| [setTopCrop(double value)](#setTopCrop-double-) | 表示裁剪矩形顶部位置，以图像高度的比例表示。 |
| [setTopCropInch(double value)](#setTopCropInch-double-) | 表示裁剪矩形顶部位置，以英寸为单位。 |
| [setTransparency(double value)](#setTransparency-double-) | 返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [setTransparentColor(CellsColor value)](#setTransparentColor-com.aspose.cells.CellsColor-) | 设置图片的透明颜色。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomCrop() {#getBottomCrop--}
```
public double getBottomCrop()
```


表示裁剪矩形底部位置，以图像高度的比例表示。

**Returns:**
double
### getBottomCropInch() {#getBottomCropInch--}
```
public double getBottomCropInch()
```


表示裁剪矩形底部位置，以英寸为单位表示。

**Returns:**
double
### getBrightness() {#getBrightness--}
```
public double getBrightness()
```


表示图片的亮度修改，以百分比为单位。

**Remarks**

范围在 -100% 到 100% 之间，工作方式与 Excel 2007 及以上版本相同。

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getContrast() {#getContrast--}
```
public double getContrast()
```


表示图片的对比度修改，以百分比为单位。

**Remarks**

范围在 -100% 到 100% 之间，工作方式与 Excel 2007 及以上版本相同。

**Returns:**
double
### getGamma() {#getGamma--}
```
public double getGamma()
```


表示图片的伽马值。

**Returns:**
double
### getLeftCrop() {#getLeftCrop--}
```
public double getLeftCrop()
```


表示裁剪矩形左侧位置，以图像宽度的比例表示。

**Returns:**
double
### getLeftCropInch() {#getLeftCropInch--}
```
public double getLeftCropInch()
```


表示裁剪矩形左侧位置，以英寸为单位。

**Returns:**
double
### getRightCrop() {#getRightCrop--}
```
public double getRightCrop()
```


表示裁剪矩形右侧位置，以图像宽度的比例表示。

**Returns:**
double
### getRightCropInch() {#getRightCropInch--}
```
public double getRightCropInch()
```


表示裁剪矩形右侧位置，以英寸为单位。

**Returns:**
double
### getTopCrop() {#getTopCrop--}
```
public double getTopCrop()
```


表示裁剪矩形顶部位置，以图像高度的比例表示。

**Returns:**
double
### getTopCropInch() {#getTopCropInch--}
```
public double getTopCropInch()
```


表示裁剪矩形顶部位置，以英寸为单位。

**Returns:**
double
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。

**Returns:**
double
### getTransparentColor() {#getTransparentColor--}
```
public CellsColor getTransparentColor()
```


获取图片的透明颜色。

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public int hashCode()
```


获取哈希码。

**Returns:**
int -
### isBiLevel() {#isBiLevel--}
```
public boolean isBiLevel()
```


指示此图片是否应以双色黑白显示。

**Returns:**
boolean
### isGray() {#isGray--}
```
public boolean isGray()
```


指示此图片是否应以灰度显示。

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




### setBiLevel(boolean value) {#setBiLevel-boolean-}
```
public void setBiLevel(boolean value)
```


指示此图片是否应以双色黑白显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBottomCrop(double value) {#setBottomCrop-double-}
```
public void setBottomCrop(double value)
```


表示裁剪矩形底部位置，以图像高度的比例表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setBottomCropInch(double value) {#setBottomCropInch-double-}
```
public void setBottomCropInch(double value)
```


表示裁剪矩形底部位置，以英寸为单位表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setBrightness(double value) {#setBrightness-double-}
```
public void setBrightness(double value)
```


表示图片的亮度修改，以百分比为单位。

**Remarks**

范围在 -100% 到 100% 之间，工作方式与 Excel 2007 及以上版本相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setContrast(double value) {#setContrast-double-}
```
public void setContrast(double value)
```


表示图片的对比度修改，以百分比为单位。

**Remarks**

范围在 -100% 到 100% 之间，工作方式与 Excel 2007 及以上版本相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setGamma(double value) {#setGamma-double-}
```
public void setGamma(double value)
```


表示图片的伽马值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setGray(boolean value) {#setGray-boolean-}
```
public void setGray(boolean value)
```


指示此图片是否应以灰度显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLeftCrop(double value) {#setLeftCrop-double-}
```
public void setLeftCrop(double value)
```


表示裁剪矩形左侧位置，以图像宽度的比例表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLeftCropInch(double value) {#setLeftCropInch-double-}
```
public void setLeftCropInch(double value)
```


表示裁剪矩形左侧位置，以英寸为单位。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setRightCrop(double value) {#setRightCrop-double-}
```
public void setRightCrop(double value)
```


表示裁剪矩形右侧位置，以图像宽度的比例表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setRightCropInch(double value) {#setRightCropInch-double-}
```
public void setRightCropInch(double value)
```


表示裁剪矩形右侧位置，以英寸为单位。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopCrop(double value) {#setTopCrop-double-}
```
public void setTopCrop(double value)
```


表示裁剪矩形顶部位置，以图像高度的比例表示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTopCropInch(double value) {#setTopCropInch-double-}
```
public void setTopCropInch(double value)
```


表示裁剪矩形顶部位置，以英寸为单位。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTransparentColor(CellsColor value) {#setTransparentColor-com.aspose.cells.CellsColor-}
```
public void setTransparentColor(CellsColor value)
```


设置图片的透明颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

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

