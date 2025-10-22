##FillFormat
Encapsulates the object that represents fill formatting for a shape.
**Inheritance:**
java.lang.Object
```
public class FillFormat
```
Encapsulates the object that represents fill formatting for a shape.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Excel object
int sheetIndex = workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a sample value to "A4" cell
worksheet.getCells().get("A4").putValue(200);
//Adding a sample value to "B1" cell
worksheet.getCells().get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.getCells().get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.getCells().get("B3").putValue(50);
//Adding a sample value to "B4" cell
worksheet.getCells().get("B4").putValue(40);
//Adding a sample value to "C1" cell as category data
worksheet.getCells().get("C1").putValue("Q1");
//Adding a sample value to "C2" cell as category data
worksheet.getCells().get("C2").putValue("Q2");
//Adding a sample value to "C3" cell as category data
worksheet.getCells().get("C3").putValue("Y1");
//Adding a sample value to "C4" cell as category data
worksheet.getCells().get("C4").putValue("Y2");
//Adding a chart to the worksheet
int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
Chart chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
int seriesIndex = chart.getNSeries().add("A1:B4", true);
//Setting the data source for the category data of NSeries
chart.getNSeries().setCategoryData("C1:C4");
//Filling the area of the 2nd NSeries with a gradient
chart.getNSeries().get(seriesIndex).getArea().getFillFormat().setOneColorGradient(Color.getLime(), 1, GradientStyleType.HORIZONTAL, 1);
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | Gets fill type |
| [getGradientColor1()](#getGradientColor1--) | Returns the gradient color 1 for the specified fill. |
| [getGradientColor2()](#getGradientColor2--) | Returns the gradient color 2 for the specified fill. |
| [getGradientColorType()](#getGradientColorType--) | Returns the gradient color type for the specified fill. |
| [getGradientDegree()](#getGradientDegree--) | Returns the gradient degree for the specified fill. |
| [getGradientFill()](#getGradientFill--) | Gets [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) object. |
| [getGradientStyle()](#getGradientStyle--) | Returns the gradient style for the specified fill. |
| [getGradientVariant()](#getGradientVariant--) | Returns the gradient variant for the specified fill. |
| [getImageData()](#getImageData--) | Gets the picture image data. |
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
| [hashCode()](#hashCode--) | Gets the hash code. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | Sets fill type |
| [setImageData(byte[] value)](#setImageData-byte---) | Sets the picture image data. |
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
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |
**Returns:**
boolean -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
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
### hashCode() {#hashCode--}
```
public int hashCode()
```
Gets the hash code.
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
