---
title: "TextBoxOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示形状的文本选项。"
type: docs
url: /zh/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

表示形状的文本选项。

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         int index = workbook.getWorksheets().get(0).getTextBoxes().add(0, 0, 350, 350);
         Shape shape = workbook.getWorksheets().get(0).getTextBoxes().get(index);
         shape.setText("This is test.");
 
         //do your business
 
         //Save the excel file.
         workbook.save("exmaple.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | 是否允许文本溢出形状。 |
| [getBottomMarginPt()](#getBottomMarginPt--) | 返回底部边距，单位为 Points。 |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | 获取左边距，单位为点。 |
| [getResizeToFitText()](#getResizeToFitText--) | 指示是否调整形状大小以适应文本 |
| [getRightMarginPt()](#getRightMarginPt--) | 获取右边距，单位为点。 |
| [getShapeTextDirection()](#getShapeTextDirection--) | 获取给定文本主体内的文本显示方向。 |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | 它对应 Excel 中的 "Format Shape - Text Options - Text Box - Vertical Alignment"。 |
| [getTopMarginPt()](#getTopMarginPt--) | 获取上边距，单位为点。 |
| [getWrapTextInShape()](#getWrapTextInShape--) | 指定形状内的文本换行。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | 是否允许文本溢出形状。 |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | 返回底部边距，单位为 Points。 |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | 设置左边距，单位为点。 |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | 指示是否调整形状大小以适应文本 |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | 设置右边距，单位为点。 |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | 设置给定文本主体内的文本显示方向。 |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | 它对应 Excel 中的 "Format Shape - Text Options - Text Box - Vertical Alignment"。 |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | 设置上边距，单位为点。 |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | 指定形状内的文本换行。 |
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
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


是否允许文本溢出形状。

**Example**

```
         shape.getTextBoxOptions().setAllowTextToOverflow(true);
```

**Returns:**
boolean
### getBottomMarginPt() {#getBottomMarginPt--}
```
public double getBottomMarginPt()
```


返回底部边距，单位为 Points。

**Example**

```
         shape.getTextBoxOptions().setBottomMarginPt(0.2d);
```

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLeftMarginPt() {#getLeftMarginPt--}
```
public double getLeftMarginPt()
```


获取左边距，单位为点。

**Example**

```
         shape.getTextBoxOptions().setLeftMarginPt(0.2d);
```

**Returns:**
double
### getResizeToFitText() {#getResizeToFitText--}
```
public boolean getResizeToFitText()
```


指示是否调整形状大小以适应文本

**Example**

```
         shape.getTextBoxOptions().setResizeToFitText(true);
```

**Returns:**
boolean
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


获取右边距，单位为点。

**Example**

```
         shape.getTextBoxOptions().setRightMarginPt(0.2d);
```

**Returns:**
double
### getShapeTextDirection() {#getShapeTextDirection--}
```
public int getShapeTextDirection()
```


获取给定文本主体内的文本显示方向。它对应于 "Format Shape - Text Options - Text Box - Text direction" 在 Excel 中。

参见 [TextVerticalType](../../com.aspose.cells/textverticaltype)。

**Example**

```
         shape.getTextBoxOptions().setShapeTextDirection(TextVerticalType.VERTICAL);
```

**Returns:**
int
### getShapeTextVerticalAlignment() {#getShapeTextVerticalAlignment--}
```
public int getShapeTextVerticalAlignment()
```


它对应 Excel 中的 "Format Shape - Text Options - Text Box - Vertical Alignment"。

参见 [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype)。

**Example**

```
         shape.getTextBoxOptions().setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


获取上边距，单位为点。

**Example**

```
         shape.getTextBoxOptions().setTopMarginPt(0.2d);
```

**Returns:**
double
### getWrapTextInShape() {#getWrapTextInShape--}
```
public boolean getWrapTextInShape()
```


指定形状内的文本换行。False - 文本主体不会换行。True - 文本主体会换行。

**Example**

```
         shape.getTextBoxOptions().setWrapTextInShape(true);
```

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




### setAllowTextToOverflow(boolean value) {#setAllowTextToOverflow-boolean-}
```
public void setAllowTextToOverflow(boolean value)
```


是否允许文本溢出形状。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


返回底部边距，单位为 Points。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


设置左边距，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


指示是否调整形状大小以适应文本

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


设置右边距，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


设置给定文本主体内的文本显示方向。它对应于 "Format Shape - Text Options - Text Box - Text direction" 在 Excel 中。

参见 [TextVerticalType](../../com.aspose.cells/textverticaltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


它对应 Excel 中的 "Format Shape - Text Options - Text Box - Vertical Alignment"。

参见 [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


设置上边距，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


指定形状内的文本换行。False - 文本主体不会换行。True - 文本主体会换行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

