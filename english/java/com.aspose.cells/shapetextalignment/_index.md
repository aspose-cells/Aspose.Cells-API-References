---
title: ShapeTextAlignment
second_title: Aspose.Cells for Java API Reference
description: Represents the setting of shapes text alignment
type: docs
weight: 509
url: /java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

Represents the setting of shape's text alignment;

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## Methods

| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether this instance has the same value as another specified [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) object. |
| [getAutoSize()](#getAutoSize--) | Indicates if size of shape is adjusted automatically according to its content. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Returns the bottom margin in unit of Points |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Returns the left margin in unit of Points |
| [getNumberOfColumns()](#getNumberOfColumns--) | Gets and sets the number of columns of text in the bounding rectangle. |
| [getRightMarginPt()](#getRightMarginPt--) | Returns the right margin in unit of Points |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Indicates whether rotating text with shape. |
| [getRotationAngle()](#getRotationAngle--) | Gets and sets the rotation of the shape. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Gets and sets the text horizontal overflow type of the text box. |
| [getTextShapeType()](#getTextShapeType--) | Gets and set the transform type of text. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Gets and sets the text vertical overflow type of the text box. |
| [getTextVerticalType()](#getTextVerticalType--) | Gets and sets the text direction. |
| [getTopMarginPt()](#getTopMarginPt--) | Returns the top margin in unit of Points |
| [hashCode()](#hashCode--) | ```
int hashCode = shapeTextAlignment.hashCode();
``` |
| [isAutoMargin()](#isAutoMargin--) | Indicates whether the margin of the text frame is automatic. |
| [isTextWrapped()](#isTextWrapped--) | Gets and sets the text wrapped type of the shape which contains text. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Please see the getter of this property: [isAutoMargin()](../../com.aspose.cells/shapetextalignment\#isAutoMargin--) |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Please see the getter of this property: [getAutoSize()](../../com.aspose.cells/shapetextalignment\#getAutoSize--) |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Please see the getter of this property: [getBottomMarginPt()](../../com.aspose.cells/shapetextalignment\#getBottomMarginPt--) |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Please see the getter of this property: [getLeftMarginPt()](../../com.aspose.cells/shapetextalignment\#getLeftMarginPt--) |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Please see the getter of this property: [getNumberOfColumns()](../../com.aspose.cells/shapetextalignment\#getNumberOfColumns--) |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Please see the getter of this property: [getRightMarginPt()](../../com.aspose.cells/shapetextalignment\#getRightMarginPt--) |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Please see the getter of this property: [getRotateTextWithShape()](../../com.aspose.cells/shapetextalignment\#getRotateTextWithShape--) |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Please see the getter of this property: [getRotationAngle()](../../com.aspose.cells/shapetextalignment\#getRotationAngle--) |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Please see the getter of this property: [getTextHorizontalOverflow()](../../com.aspose.cells/shapetextalignment\#getTextHorizontalOverflow--) |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Please see the getter of this property: [getTextShapeType()](../../com.aspose.cells/shapetextalignment\#getTextShapeType--) |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Please see the getter of this property: [getTextVerticalOverflow()](../../com.aspose.cells/shapetextalignment\#getTextVerticalOverflow--) |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Please see the getter of this property: [getTextVerticalType()](../../com.aspose.cells/shapetextalignment\#getTextVerticalType--) |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Please see the getter of this property: [isTextWrapped()](../../com.aspose.cells/shapetextalignment\#isTextWrapped--) |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Please see the getter of this property: [getTopMarginPt()](../../com.aspose.cells/shapetextalignment\#getTopMarginPt--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether this instance has the same value as another specified [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) object.

```
//You have to make sure that the index value in this line of code exists
         ShapeTextAlignment obj = workbook.getWorksheets().get(0).getShapes().get(0).getTextBody().getTextAlignment();
         if (shapeTextAlignment.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) object to compare with this instance. |

**Returns:**
boolean - true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


Indicates if size of shape is adjusted automatically according to its content.

```
shapeTextAlignment.setAutoSize(false);
```

**Returns:**
boolean
### getBottomMarginPt() {#getBottomMarginPt--}
```
public double getBottomMarginPt()
```


Returns the bottom margin in unit of Points

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


Returns the left margin in unit of Points

```
shapeTextAlignment.setLeftMarginPt(2.0d);
```

**Returns:**
double
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


Gets and sets the number of columns of text in the bounding rectangle.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


Returns the right margin in unit of Points

```
shapeTextAlignment.setRightMarginPt(2.0d);
```

**Returns:**
double
### getRotateTextWithShape() {#getRotateTextWithShape--}
```
public boolean getRotateTextWithShape()
```


Indicates whether rotating text with shape.

```
shapeTextAlignment.setRotateTextWithShape(true);
```

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


Gets and sets the rotation of the shape.

```
shapeTextAlignment.setRotationAngle(90);
```

**Returns:**
double
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


Gets and sets the text horizontal overflow type of the text box.

```
shapeTextAlignment.setTextHorizontalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


Gets and set the transform type of text.

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


Gets and sets the text vertical overflow type of the text box.

```
shapeTextAlignment.setTextVerticalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextVerticalType() {#getTextVerticalType--}
```
public int getTextVerticalType()
```


Gets and sets the text direction.

```
shapeTextAlignment.setTextVerticalType(com.aspose.cells.TextVerticalType.HORIZONTAL);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


Returns the top margin in unit of Points

```
shapeTextAlignment.setTopMarginPt(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


```
int hashCode = shapeTextAlignment.hashCode();
```

**Returns:**
int - 
### isAutoMargin() {#isAutoMargin--}
```
public boolean isAutoMargin()
```


Indicates whether the margin of the text frame is automatic.

```
shapeTextAlignment.setAutoMargin(true);
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Gets and sets the text wrapped type of the shape which contains text.

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


Please see the getter of this property: [isAutoMargin()](../../com.aspose.cells/shapetextalignment\#isAutoMargin--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


Please see the getter of this property: [getAutoSize()](../../com.aspose.cells/shapetextalignment\#getAutoSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


Please see the getter of this property: [getBottomMarginPt()](../../com.aspose.cells/shapetextalignment\#getBottomMarginPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


Please see the getter of this property: [getLeftMarginPt()](../../com.aspose.cells/shapetextalignment\#getLeftMarginPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


Please see the getter of this property: [getNumberOfColumns()](../../com.aspose.cells/shapetextalignment\#getNumberOfColumns--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


Please see the getter of this property: [getRightMarginPt()](../../com.aspose.cells/shapetextalignment\#getRightMarginPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


Please see the getter of this property: [getRotateTextWithShape()](../../com.aspose.cells/shapetextalignment\#getRotateTextWithShape--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Please see the getter of this property: [getRotationAngle()](../../com.aspose.cells/shapetextalignment\#getRotationAngle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Please see the getter of this property: [getTextHorizontalOverflow()](../../com.aspose.cells/shapetextalignment\#getTextHorizontalOverflow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Please see the getter of this property: [getTextShapeType()](../../com.aspose.cells/shapetextalignment\#getTextShapeType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Please see the getter of this property: [getTextVerticalOverflow()](../../com.aspose.cells/shapetextalignment\#getTextVerticalOverflow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


Please see the getter of this property: [getTextVerticalType()](../../com.aspose.cells/shapetextalignment\#getTextVerticalType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Please see the getter of this property: [isTextWrapped()](../../com.aspose.cells/shapetextalignment\#isTextWrapped--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


Please see the getter of this property: [getTopMarginPt()](../../com.aspose.cells/shapetextalignment\#getTopMarginPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

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

