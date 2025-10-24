##GradientFill
Represents the gradient fill.
**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```
Represents the gradient fill.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | The angle of linear fill. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Gets the gradient direction type. |
| [getFillType()](#getFillType--) | Gets the gradient fill type. |
| [getGradientColor1()](#getGradientColor1--) | Gets gradient color 1. |
| [getGradientColor2()](#getGradientColor2--) | Gets gradient color 2. |
| [getGradientColorType()](#getGradientColorType--) | Gets gradient color type. |
| [getGradientDegree()](#getGradientDegree--) | Gets gradient degree. |
| [getGradientStops()](#getGradientStops--) | Represents the gradient stop collection. |
| [getGradientStyle()](#getGradientStyle--) | Gets gradient style type. |
| [getPresetColor()](#getPresetColor--) | Returns the gradient preset color for the specified fill. |
| [getVariant()](#getVariant--) | Gets variant. |
| [hashCode()](#hashCode--) | Gets the hash code. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | The angle of linear fill. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Set the gradient fill type and direction. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Sets the specified fill to a one-color gradient. |
| [setPresetColor(int value)](#setPresetColor-int-) | Returns the gradient preset color for the specified fill. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Sets the specified fill to a preset-color gradient. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Sets preset theme gradient fill. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Sets the specified fill to a two-color gradient. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Sets the specified fill to a two-color gradient. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
/
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |
**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```
The angle of linear fill.
**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```
Gets the gradient direction type.
See [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).
**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```
Gets the gradient fill type.
See [GradientFillType](../../com.aspose.cells/gradientfilltype).
**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```
Gets gradient color 1. Applies to Excel97-2003
**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```
Gets gradient color 2. Applies to Excel97-2003
**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```
Gets gradient color type. Applies to Excel97-2003
See [GradientColorType](../../com.aspose.cells/gradientcolortype).
**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```
Gets gradient degree. Applies to Excel97-2003
**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```
Represents the gradient stop collection.
**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```
Gets gradient style type. Applies to Excel97-2003
See [GradientStyleType](../../com.aspose.cells/gradientstyletype).
**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```
Returns the gradient preset color for the specified fill. Applies to Excel97-2003
See [GradientPresetType](../../com.aspose.cells/gradientpresettype).
**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```
Gets variant. Applies to Excel97-2003
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
### setAngle(float value) {#setAngle-float-}
```
public void setAngle(float value)
```
The angle of linear fill.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | float |  |
### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```
Set the gradient fill type and direction.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Gradient fill type. |
| angle | double | The angle. Only applies for GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). The direction type. Only applies for GradientFillType.Radial and GradientFillType.Rectangle. |
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
### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```
Returns the gradient preset color for the specified fill. Applies to Excel97-2003
See [GradientPresetType](../../com.aspose.cells/gradientpresettype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```
Sets the specified fill to a preset-color gradient. Only applies for Excel 97-2003
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Preset color type |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```
Sets preset theme gradient fill.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). The preset gradient type. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). The theme color type. |
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
