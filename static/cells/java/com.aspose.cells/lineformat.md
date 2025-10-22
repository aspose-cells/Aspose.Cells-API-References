##LineFormat
Represents all setting of the line.
**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```
Represents all setting of the line.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.getLine();
//do your business
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether this instance has the same value as another specified [LineFormat](../../com.aspose.cells/lineformat) object. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Gets the begin arrow length type of the line. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Gets the begin arrow type of the line. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Gets the begin arrow width type of the line. |
| [getCapType()](#getCapType--) | Specifies the ending caps. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Specifies the line compound type. |
| [getDashStyle()](#getDashStyle--) | Specifies the line dash type. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Gets the end arrow length type of the line. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Gets the end arrow type of the line. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Gets the end arrow width type of the line. |
| [getFillType()](#getFillType--) | Gets fill type |
| [getGradientColor1()](#getGradientColor1--) | Returns the gradient color 1 for the specified fill. |
| [getGradientColor2()](#getGradientColor2--) | Returns the gradient color 2 for the specified fill. |
| [getGradientColorType()](#getGradientColorType--) | Returns the gradient color type for the specified fill. |
| [getGradientDegree()](#getGradientDegree--) | Returns the gradient degree for the specified fill. |
| [getGradientFill()](#getGradientFill--) | Gets [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) object. |
| [getGradientStyle()](#getGradientStyle--) | Returns the gradient style for the specified fill. |
| [getGradientVariant()](#getGradientVariant--) | Returns the gradient variant for the specified fill. |
| [getImageData()](#getImageData--) | Gets the picture image data. |
| [getJoinType()](#getJoinType--) | Specifies the line join type. |
| [getPattern()](#getPattern--) | Represents an area's display pattern. |
| [getPatternFill()](#getPatternFill--) | Gets [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) object. |
| [getPictureFormatType()](#getPictureFormatType--) | Gets the picture format type. |
| [getPresetColor()](#getPresetColor--) | Returns the gradient preset color for the specified fill. |
| [getScale()](#getScale--) | Gets the picture format scale. |
| [getSetType()](#getSetType--) | Gets the fill format set type. |
| [getSolidFill()](#getSolidFill--) | Gets [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) object. |
| [getTexture()](#getTexture--) | Represents the texture type for the specified fill. |
| [getTextureFill()](#getTextureFill--) | Gets [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) object. |
| [getTransparency()](#getTransparency--) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#getType--) | Gets the fill type. |
| [getWeight()](#getWeight--) | Gets the weight of the line in unit of points. |
| [hashCode()](#hashCode--) | Gets the hash code. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Sets the begin arrow length type of the line. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Sets the begin arrow type of the line. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Sets the begin arrow width type of the line. |
| [setCapType(int value)](#setCapType-int-) | Specifies the ending caps. |
| [setCompoundType(int value)](#setCompoundType-int-) | Specifies the line compound type. |
| [setDashStyle(int value)](#setDashStyle-int-) | Specifies the line dash type. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Sets the end arrow length type of the line. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Sets the end arrow type of the line. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Sets the end arrow width type of the line. |
| [setFillType(int value)](#setFillType-int-) | Sets fill type |
| [setImageData(byte[] value)](#setImageData-byte---) | Sets the picture image data. |
| [setJoinType(int value)](#setJoinType-int-) | Specifies the line join type. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Sets the specified fill to a one-color gradient. |
| [setPattern(int value)](#setPattern-int-) | Represents an area's display pattern. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Sets the picture format type. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Sets the specified fill to a preset-color gradient. |
| [setScale(double value)](#setScale-double-) | Sets the picture format scale. |
| [setSetType(int value)](#setSetType-int-) | Gets the fill format set type. |
| [setTexture(int value)](#setTexture-int-) | Represents the texture type for the specified fill. |
| [setTransparency(double value)](#setTransparency-double-) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Sets the specified fill to a two-color gradient. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Sets the specified fill to a two-color gradient. |
| [setType(int value)](#setType-int-) | Sets the fill type. |
| [setWeight(double value)](#setWeight-double-) | Sets the weight of the line in unit of points. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
Determines whether this instance has the same value as another specified [LineFormat](../../com.aspose.cells/lineformat) object.
**Example**
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
Gets the begin arrow length type of the line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Example**
```
lineFmt.setBeginArrowheadLength(MsoArrowheadLength.LONG);
```
**Returns:**
int
### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}
```
public int getBeginArrowheadStyle()
```
Gets the begin arrow type of the line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Example**
```
lineFmt.setBeginArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```
**Returns:**
int
### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}
```
public int getBeginArrowheadWidth()
```
Gets the begin arrow width type of the line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Example**
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
See [LineCapType](../../com.aspose.cells/linecaptype).
**Example**
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
See [MsoLineStyle](../../com.aspose.cells/msolinestyle).
**Example**
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
See [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).
**Example**
```
lineFmt.setDashStyle(MsoLineDashStyle.SOLID);
```
**Returns:**
int
### getEndArrowheadLength() {#getEndArrowheadLength--}
```
public int getEndArrowheadLength()
```
Gets the end arrow length type of the line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Example**
```
lineFmt.setEndArrowheadLength(MsoArrowheadLength.LONG);
```
**Returns:**
int
### getEndArrowheadStyle() {#getEndArrowheadStyle--}
```
public int getEndArrowheadStyle()
```
Gets the end arrow type of the line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Example**
```
lineFmt.setEndArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```
**Returns:**
int
### getEndArrowheadWidth() {#getEndArrowheadWidth--}
```
public int getEndArrowheadWidth()
```
Gets the end arrow width type of the line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Example**
```
lineFmt.setEndArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```
**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```
Gets fill type
See [FillType](../../com.aspose.cells/filltype).
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
Returns the gradient color 2 for the specified fill.
**Remarks**
Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.
**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```
Returns the gradient color type for the specified fill.
See [GradientColorType](../../com.aspose.cells/gradientcolortype).
**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```
Returns the gradient degree for the specified fill. Only applies for Excel 2007.
**Remarks**
Can only be a value from 0.0 (dark) through 1.0 (light).
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
See [GradientStyleType](../../com.aspose.cells/gradientstyletype).
**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```
Returns the gradient variant for the specified fill. Only applies for Excel 2007.
**Remarks**
Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.
**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```
Gets the picture image data.
**Remarks**
If the fill format is not custom texture format, returns null.
**Returns:**
byte[]
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```
Specifies the line join type.
See [LineJoinType](../../com.aspose.cells/linejointype).
**Example**
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
See [FillPattern](../../com.aspose.cells/fillpattern).
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
Gets the picture format type.
See [FillPictureType](../../com.aspose.cells/fillpicturetype).
**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```
Returns the gradient preset color for the specified fill.
See [GradientPresetType](../../com.aspose.cells/gradientpresettype).
**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```
Gets the picture format scale.
**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```
Gets the fill format set type.
See [FormatSetType](../../com.aspose.cells/formatsettype).
**Remarks**
NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.
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
See [TextureType](../../com.aspose.cells/texturetype).
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
Gets the fill type.
See [FillType](../../com.aspose.cells/filltype).
**Remarks**
NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getWeight() {#getWeight--}
```
public double getWeight()
```
Gets the weight of the line in unit of points.
**Example**
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
**Example**
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
Sets the begin arrow length type of the line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```
Sets the begin arrow type of the line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```
Sets the begin arrow width type of the line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```
Specifies the ending caps.
See [LineCapType](../../com.aspose.cells/linecaptype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```
Specifies the line compound type.
See [MsoLineStyle](../../com.aspose.cells/msolinestyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```
Specifies the line dash type.
See [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```
Sets the end arrow length type of the line.
See [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```
Sets the end arrow type of the line.
See [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```
Sets the end arrow width type of the line.
See [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```
Sets fill type
See [FillType](../../com.aspose.cells/filltype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```
Sets the picture image data.
**Remarks**
If the fill format is not custom texture format, returns null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |
### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```
Specifies the line join type.
See [LineJoinType](../../com.aspose.cells/linejointype).
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
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```
Represents an area's display pattern.
See [FillPattern](../../com.aspose.cells/fillpattern).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```
Sets the picture format type.
See [FillPictureType](../../com.aspose.cells/fillpicturetype).
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
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Preset color type |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```
Sets the picture format scale.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```
Gets the fill format set type.
See [FormatSetType](../../com.aspose.cells/formatsettype).
**Remarks**
NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```
Represents the texture type for the specified fill.
See [TextureType](../../com.aspose.cells/texturetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
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
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient shading style. |
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
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setType(int value) {#setType-int-}
```
public void setType(int value)
```
Sets the fill type.
See [FillType](../../com.aspose.cells/filltype).
**Remarks**
NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```
Sets the weight of the line in unit of points.
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
