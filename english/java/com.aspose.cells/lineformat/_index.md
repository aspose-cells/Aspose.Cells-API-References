---
title: LineFormat
second_title: Aspose.Cells for Java API Reference
description: Represents all setting of the line.
type: docs
weight: 297
url: /java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Represents all setting of the line.

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Constructors

| Constructor | Description |
| --- | --- |
| [LineFormat()](#LineFormat--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether this instance has the same value as another specified [LineFormat](../../com.aspose.cells/lineformat) object. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Gets and sets the begin arrow length type of the line. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Gets and sets the begin arrow type of the line. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Gets and sets the begin arrow width type of the line. |
| [getCapType()](#getCapType--) | Specifies the ending caps. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Specifies the line compound type. |
| [getDashStyle()](#getDashStyle--) | Specifies the line dash type. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Gets and sets the end arrow length type of the line. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Gets and sets the end arrow type of the line. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Gets and sets the end arrow width type of the line. |
| [getFillType()](#getFillType--) | Gets and sets fill type |
| [getGradientColor1()](#getGradientColor1--) | Returns the gradient color 1 for the specified fill. |
| [getGradientColor2()](#getGradientColor2--) | Returns the gradient color 2 for the specified fill. |
| [getGradientColorType()](#getGradientColorType--) | Returns the gradient color type for the specified fill. |
| [getGradientDegree()](#getGradientDegree--) | Returns the gradient degree for the specified fill. |
| [getGradientFill()](#getGradientFill--) | Gets [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) object. |
| [getGradientStyle()](#getGradientStyle--) | Returns the gradient style for the specified fill. |
| [getGradientVariant()](#getGradientVariant--) | Returns the gradient variant for the specified fill. |
| [getImageData()](#getImageData--) | Gets and sets the picture image data. |
| [getJoinType()](#getJoinType--) | Specifies the line join type. |
| [getPattern()](#getPattern--) | Represents an area's display pattern. |
| [getPatternFill()](#getPatternFill--) | Gets [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) object. |
| [getPictureFormatType()](#getPictureFormatType--) | Gets and sets the picture format type. |
| [getPresetColor()](#getPresetColor--) | Returns the gradient preset color for the specified fill. |
| [getScale()](#getScale--) | Gets and sets the picture format scale. |
| [getSetType()](#getSetType--) | Gets the fill format set type. |
| [getSolidFill()](#getSolidFill--) | Gets [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) object. |
| [getTexture()](#getTexture--) | Represents the texture type for the specified fill. |
| [getTextureFill()](#getTextureFill--) | Gets [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) object. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#getType--) | Gets and sets the fill type. |
| [getWeight()](#getWeight--) | Gets or sets the weight of the line in unit of points. |
| [hashCode()](#hashCode--) | Gets the hash code. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | For the description of this property, please see \#getBeginArrowheadLength().getBeginArrowheadLength() |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | For the description of this property, please see \#getBeginArrowheadStyle().getBeginArrowheadStyle() |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | For the description of this property, please see \#getBeginArrowheadWidth().getBeginArrowheadWidth() |
| [setCapType(int value)](#setCapType-int-) | For the description of this property, please see \#getCapType().getCapType() |
| [setCompoundType(int value)](#setCompoundType-int-) | For the description of this property, please see \#getCompoundType().getCompoundType() |
| [setDashStyle(int value)](#setDashStyle-int-) | For the description of this property, please see \#getDashStyle().getDashStyle() |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | For the description of this property, please see \#getEndArrowheadLength().getEndArrowheadLength() |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | For the description of this property, please see \#getEndArrowheadStyle().getEndArrowheadStyle() |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | For the description of this property, please see \#getEndArrowheadWidth().getEndArrowheadWidth() |
| [setFillType(int value)](#setFillType-int-) | For the description of this property, please see \#getFillType().getFillType() |
| [setImageData(byte[] value)](#setImageData-byte---) | For the description of this property, please see \#getImageData().getImageData() |
| [setJoinType(int value)](#setJoinType-int-) | For the description of this property, please see \#getJoinType().getJoinType() |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Sets the specified fill to a one-color gradient. |
| [setPattern(int value)](#setPattern-int-) | For the description of this property, please see \#getPattern().getPattern() |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | For the description of this property, please see \#getPictureFormatType().getPictureFormatType() |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Sets the specified fill to a preset-color gradient. |
| [setScale(double value)](#setScale-double-) | For the description of this property, please see \#getScale().getScale() |
| [setSetType(int value)](#setSetType-int-) | For the description of this property, please see \#getSetType().getSetType() |
| [setTexture(int value)](#setTexture-int-) | For the description of this property, please see \#getTexture().getTexture() |
| [setTransparency(double value)](#setTransparency-double-) | For the description of this property, please see \#getTransparency().getTransparency() |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Sets the specified fill to a two-color gradient. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Sets the specified fill to a two-color gradient. |
| [setType(int value)](#setType-int-) | For the description of this property, please see \#getType().getType() |
| [setWeight(double value)](#setWeight-double-) | For the description of this property, please see \#getWeight().getWeight() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LineFormat() {#LineFormat--}
```
public LineFormat()
```


### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determines whether this instance has the same value as another specified [LineFormat](../../com.aspose.cells/lineformat) object.

```
//You have to make sure that the index value in this line of code exists
         LineFormat obj = workbook.getWorksheets().get(0).getShapes().get(0).getLine();
         if (lineFmt.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The [LineFormat](../../com.aspose.cells/lineformat) object to compare with this instance. |

**Returns:**
boolean - true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Gets and sets the begin arrow length type of the line.

```
lineFmt.setBeginArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}
```
public int getBeginArrowheadStyle()
```


Gets and sets the begin arrow type of the line.

```
lineFmt.setBeginArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}
```
public int getBeginArrowheadWidth()
```


Gets and sets the begin arrow width type of the line.

```
lineFmt.setBeginArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Specifies the ending caps.

```
lineFmt.setCapType(LineCapType.FLAT);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Specifies the line compound type.

```
lineFmt.setCompoundType(MsoLineStyle.SINGLE);
```

**Returns:**
int
### getDashStyle() {#getDashStyle--}
```
public int getDashStyle()
```


Specifies the line dash type.

```
lineFmt.setDashStyle(MsoLineDashStyle.SOLID);
```

**Returns:**
int
### getEndArrowheadLength() {#getEndArrowheadLength--}
```
public int getEndArrowheadLength()
```


Gets and sets the end arrow length type of the line.

```
lineFmt.setEndArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getEndArrowheadStyle() {#getEndArrowheadStyle--}
```
public int getEndArrowheadStyle()
```


Gets and sets the end arrow type of the line.

```
lineFmt.setEndArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getEndArrowheadWidth() {#getEndArrowheadWidth--}
```
public int getEndArrowheadWidth()
```


Gets and sets the end arrow width type of the line.

```
lineFmt.setEndArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Gets and sets fill type

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Returns the gradient color 1 for the specified fill.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Returns the gradient color 2 for the specified fill. Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Returns the gradient color type for the specified fill.

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Returns the gradient degree for the specified fill. Only applies for Excel 2007. Can only be a value from 0.0 (dark) through 1.0 (light).

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Gets [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) object.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Returns the gradient style for the specified fill.

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Returns the gradient variant for the specified fill. Only applies for Excel 2007. Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Gets and sets the picture image data. If the fill format is not custom texture format, returns null.

**Returns:**
byte[]
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Specifies the line join type.

```
lineFmt.setJoinType(LineJoinType.ROUND);
```

**Returns:**
int
### getPattern() {#getPattern--}
```
public int getPattern()
```


Represents an area's display pattern.

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Gets [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) object.

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Gets and sets the picture format type.

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Returns the gradient preset color for the specified fill.

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Gets and sets the picture format scale.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Gets the fill format set type. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Gets [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) object.

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Represents the texture type for the specified fill.

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Gets [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) object.

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Gets and sets the fill type. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getWeight() {#getWeight--}
```
public double getWeight()
```


Gets or sets the weight of the line in unit of points.

```
lineFmt.setWeight(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gets the hash code.

```
int hashCode = lineFmt.hashCode();
```

**Returns:**
int - 
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBeginArrowheadLength(int value) {#setBeginArrowheadLength-int-}
```
public void setBeginArrowheadLength(int value)
```


For the description of this property, please see \#getBeginArrowheadLength().getBeginArrowheadLength()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


For the description of this property, please see \#getBeginArrowheadStyle().getBeginArrowheadStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


For the description of this property, please see \#getBeginArrowheadWidth().getBeginArrowheadWidth()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


For the description of this property, please see \#getCapType().getCapType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


For the description of this property, please see \#getCompoundType().getCompoundType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


For the description of this property, please see \#getDashStyle().getDashStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


For the description of this property, please see \#getEndArrowheadLength().getEndArrowheadLength()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


For the description of this property, please see \#getEndArrowheadStyle().getEndArrowheadStyle()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


For the description of this property, please see \#getEndArrowheadWidth().getEndArrowheadWidth()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


For the description of this property, please see \#getFillType().getFillType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


For the description of this property, please see \#getImageData().getImageData()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


For the description of this property, please see \#getJoinType().getJoinType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | One gradient color. |
| degree | double | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | int | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


For the description of this property, please see \#getPattern().getPattern()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


For the description of this property, please see \#getPictureFormatType().getPictureFormatType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Sets the specified fill to a preset-color gradient. Only applies for Excel 2007.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | int | Preset color type |
| style | int | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


For the description of this property, please see \#getScale().getScale()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


For the description of this property, please see \#getSetType().getSetType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


For the description of this property, please see \#getTexture().getTexture()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


For the description of this property, please see \#getTransparency().getTransparency()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | One gradient color. |
| color2 | [Color](../../com.aspose.cells/color) | Two gradient color. |
| style | int | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | One gradient color. |
| transparency1 | double | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | [Color](../../com.aspose.cells/color) | Two gradient color. |
| transparency2 | double | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | int | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


For the description of this property, please see \#getType().getType()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


For the description of this property, please see \#getWeight().getWeight()

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

