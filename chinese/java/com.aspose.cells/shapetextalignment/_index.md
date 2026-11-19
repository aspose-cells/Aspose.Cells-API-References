---
title: "ShapeTextAlignment"
second_title: "Aspose.Cells for Java API 参考"
description: "表示形状文本对齐的设置"
type: docs
url: /zh/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

表示形状文本对齐的设置；

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | 确定此实例是否与另一个指定的 [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) 对象具有相同的值。 |
| [getAutoSize()](#getAutoSize--) | 指示形状的大小是否根据其内容自动调整。 |
| [getBottomMarginPt()](#getBottomMarginPt--) | 返回底部边距，单位为 Points。 |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | 返回左侧边距，单位为 Points。 |
| [getNumberOfColumns()](#getNumberOfColumns--) | 获取边界矩形中文本的列数。 |
| [getRightMarginPt()](#getRightMarginPt--) | 返回右侧边距，单位为 Points。 |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | 指示是否随形状旋转文本。 |
| [getRotationAngle()](#getRotationAngle--) | 获取形状的旋转角度。 |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | 获取文本框中文本水平溢出类型。 |
| [getTextShapeType()](#getTextShapeType--) | 获取文本的变换类型。 |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | 获取文本框中文本垂直溢出类型。 |
| [getTextVerticalType()](#getTextVerticalType--) | 获取文本方向。 |
| [getTopMarginPt()](#getTopMarginPt--) | 返回顶部边距，单位为 Points。 |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | 指示文本框的边距是否为自动。 |
| [isLockedText()](#isLockedText--) | 指示在工作表受保护时形状是否被锁定。 |
| [isTextWrapped()](#isTextWrapped--) | 获取包含文本的形状的文本换行类型。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | 指示文本框的边距是否为自动。 |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | 指示形状的大小是否根据其内容自动调整。 |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | 返回底部边距，单位为 Points。 |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | 返回左侧边距，单位为 Points。 |
| [setLockedText(boolean value)](#setLockedText-boolean-) | 指示在工作表受保护时形状是否被锁定。 |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | 设置边界矩形中文本的列数。 |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | 返回右侧边距，单位为 Points。 |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | 指示是否随形状旋转文本。 |
| [setRotationAngle(double value)](#setRotationAngle-double-) | 设置形状的旋转角度。 |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | 设置文本框中文本水平溢出类型。 |
| [setTextShapeType(int value)](#setTextShapeType-int-) | 设置文本的变换类型。 |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | 设置文本框中文本垂直溢出类型。 |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | 设置文本方向。 |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | 设置包含文本的形状的文本换行类型。 |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | 返回顶部边距，单位为 Points。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


确定此实例是否与另一个指定的 [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) 对象具有相同的值。

**Example**

```
         //You have to make sure that the index value in this line of code exists
         ShapeTextAlignment obj = workbook.getWorksheets().get(0).getShapes().get(0).getTextBody().getTextAlignment();
         if (shapeTextAlignment.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| obj | java.lang.Object | 用于与此实例比较的 [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) 对象。 |

**Returns:**
boolean - 如果 obj 参数的值与此实例的值相同，则为 true；否则为 false。如果 obj 为 null，则此方法返回 false。
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


指示形状的大小是否根据其内容自动调整。

**Example**

```
         shapeTextAlignment.setAutoSize(false);
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
         shapeTextAlignment.setBottomMarginPt(2.0d);
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


返回左侧边距，单位为 Points。

**Example**

```
         shapeTextAlignment.setLeftMarginPt(2.0d);
```

**Returns:**
double
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


获取边界矩形中文本的列数。

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


返回右侧边距，单位为 Points。

**Example**

```
         shapeTextAlignment.setRightMarginPt(2.0d);
```

**Returns:**
double
### getRotateTextWithShape() {#getRotateTextWithShape--}
```
public boolean getRotateTextWithShape()
```


指示是否随形状旋转文本。

**Example**

```
         shapeTextAlignment.setRotateTextWithShape(true);
```

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


获取形状的旋转角度。

**Example**

```
         shapeTextAlignment.setRotationAngle(90);
```

**Returns:**
double
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


获取文本框中文本水平溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Example**

```
         shapeTextAlignment.setTextHorizontalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


获取文本的变换类型。

参见 [AutoShapeType](../../com.aspose.cells/autoshapetype)。

**Example**

```
         //Usually do not modify this value unless you know exactly what the modification will result in
         shapeTextAlignment.setTextShapeType(AutoShapeType.TEXT_BOX);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


获取文本框中文本垂直溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Example**

```
         shapeTextAlignment.setTextVerticalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextVerticalType() {#getTextVerticalType--}
```
public int getTextVerticalType()
```


获取文本方向。

参见 [TextVerticalType](../../com.aspose.cells/textverticaltype)。

**Example**

```
         shapeTextAlignment.setTextVerticalType(com.aspose.cells.TextVerticalType.HORIZONTAL);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


返回顶部边距，单位为 Points。

**Example**

```
         shapeTextAlignment.setTopMarginPt(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### isAutoMargin() {#isAutoMargin--}
```
public boolean isAutoMargin()
```


指示文本框的边距是否为自动。

**Example**

```
         shapeTextAlignment.setAutoMargin(true);
```

**Returns:**
boolean
### isLockedText() {#isLockedText--}
```
public boolean isLockedText()
```


指示在工作表受保护时形状是否被锁定。

**Remarks**

仅在工作表受保护时有效。

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


获取包含文本的形状的文本换行类型。

**Example**

```
         shapeTextAlignment.setTextWrapped(true);
```

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




### setAutoMargin(boolean value) {#setAutoMargin-boolean-}
```
public void setAutoMargin(boolean value)
```


指示文本框的边距是否为自动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


指示形状的大小是否根据其内容自动调整。

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


返回左侧边距，单位为 Points。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


指示在工作表受保护时形状是否被锁定。

**Remarks**

仅在工作表受保护时有效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


设置边界矩形中文本的列数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


返回右侧边距，单位为 Points。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


指示是否随形状旋转文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


设置形状的旋转角度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


设置文本框中文本水平溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


设置文本的变换类型。

参见 [AutoShapeType](../../com.aspose.cells/autoshapetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


设置文本框中文本垂直溢出类型。

参见 [TextOverflowType](../../com.aspose.cells/textoverflowtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


设置文本方向。

参见 [TextVerticalType](../../com.aspose.cells/textverticaltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


设置包含文本的形状的文本换行类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


返回顶部边距，单位为 Points。

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

