---
title: "FillFormat"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示形状填充格式的对象。"
type: docs
url: /zh/java/com.aspose.cells/fillformat/
---

**Inheritance:**
java.lang.Object
```
public class FillFormat
```

封装表示形状填充格式的对象。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | 获取填充类型 |
| [getGradientColor1()](#getGradientColor1--) | 返回指定填充的渐变颜色 1。 |
| [getGradientColor2()](#getGradientColor2--) | 返回指定填充的渐变颜色 2。 |
| [getGradientColorType()](#getGradientColorType--) | 返回指定填充的渐变颜色类型。 |
| [getGradientDegree()](#getGradientDegree--) | 返回指定填充的渐变角度。 |
| [getGradientFill()](#getGradientFill--) | 获取 [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) 对象。 |
| [getGradientStyle()](#getGradientStyle--) | 返回指定填充的渐变样式。 |
| [getGradientVariant()](#getGradientVariant--) | 返回指定填充的渐变变体。 |
| [getImageData()](#getImageData--) | 获取图片图像数据。 |
| [getPattern()](#getPattern--) | 表示区域的显示模式。 |
| [getPatternFill()](#getPatternFill--) | 获取 [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) 对象。 |
| [getPictureFormatType()](#getPictureFormatType--) | 获取图片格式类型。 |
| [getPresetColor()](#getPresetColor--) | 返回指定填充的渐变预设颜色。 |
| [getScale()](#getScale--) | 获取图片格式比例。 |
| [getSetType()](#getSetType--) | 获取填充格式设置类型。 |
| [getSolidFill()](#getSolidFill--) | 获取 [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) 对象。 |
| [getTexture()](#getTexture--) | 表示指定填充的纹理类型。 |
| [getTextureFill()](#getTextureFill--) | 获取 [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) 对象。 |
| [getTransparency()](#getTransparency--) | 返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [getType()](#getType--) | 获取填充类型。 |
| [hashCode()](#hashCode--) | 获取哈希码。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | 设置填充类型 |
| [setImageData(byte[] value)](#setImageData-byte---) | 设置图片图像数据。 |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | 将指定填充设置为单色渐变。 |
| [setPattern(int value)](#setPattern-int-) | 表示区域的显示模式。 |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | 设置图片格式类型。 |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | 将指定填充设置为预设颜色渐变。 |
| [setScale(double value)](#setScale-double-) | 设置图片格式比例。 |
| [setSetType(int value)](#setSetType-int-) | 获取填充格式设置类型。 |
| [setTexture(int value)](#setTexture-int-) | 表示指定填充的纹理类型。 |
| [setTransparency(double value)](#setTransparency-double-) | 返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。 |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | 将指定填充设置为双色渐变。 |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | 将指定填充设置为双色渐变。 |
| [setType(int value)](#setType-int-) | 设置填充类型。 |
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


获取填充类型

参见 [FillType](../../com.aspose.cells/filltype)。

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


返回指定填充的渐变颜色 1。

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


返回指定填充的渐变颜色 2。

**Remarks**

仅当渐变颜色类型为 GradientColorType.TwoColors 时，此属性才有意义。

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


返回指定填充的渐变颜色类型。

参见 [GradientColorType](../../com.aspose.cells/gradientcolortype)。

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


返回指定填充的渐变程度。仅适用于 Excel 2007。

**Remarks**

只能取 0.0（暗）到 1.0（亮）之间的值。

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


获取 [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) 对象。

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


返回指定填充的渐变样式。

参见 [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


返回指定填充的渐变变体。仅适用于 Excel 2007。

**Remarks**

只能取 1 到 4 之间的值，对应“填充效果”对话框中“渐变”选项卡的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


获取图片图像数据。

**Remarks**

如果填充格式不是自定义纹理格式，则返回 null。

**Returns:**
byte[]
### getPattern() {#getPattern--}
```
public int getPattern()
```


表示区域的显示模式。

参见 [FillPattern](../../com.aspose.cells/fillpattern)。

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


获取 [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) 对象。

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


获取图片格式类型。

请参阅 [FillPictureType](../../com.aspose.cells/fillpicturetype)。

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


返回指定填充的渐变预设颜色。

参见 [GradientPresetType](../../com.aspose.cells/gradientpresettype)。

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


获取图片格式比例。

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


获取填充格式设置类型。

请参阅 [FormatSetType](../../com.aspose.cells/formatsettype)。

**Remarks**

注意：此成员现已过时。请改用 FillFormat.FillType 属性。此属性将在自 2016 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


获取 [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) 对象。

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


表示指定填充的纹理类型。

参见 [TextureType](../../com.aspose.cells/texturetype)。

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


获取 [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) 对象。

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


获取填充类型。

参见 [FillType](../../com.aspose.cells/filltype)。

**Remarks**

注意：此成员现已过时。请改用 FillFormat.FillType 属性。此属性将在自 2016 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


获取哈希码。

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


设置填充类型

参见 [FillType](../../com.aspose.cells/filltype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


设置图片图像数据。

**Remarks**

如果填充格式不是自定义纹理格式，则返回 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


将指定的填充设置为单色渐变。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| degree | double | 渐变的度数。取值范围为 0.0（暗）至 1.0（亮）。 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


表示区域的显示模式。

参见 [FillPattern](../../com.aspose.cells/fillpattern)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


设置图片格式类型。

请参阅 [FillPictureType](../../com.aspose.cells/fillpicturetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


将指定的填充设置为预设颜色渐变。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype)。预设颜色类型 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


设置图片格式比例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


获取填充格式设置类型。

请参阅 [FormatSetType](../../com.aspose.cells/formatsettype)。

**Remarks**

注意：此成员现已过时。请改用 FillFormat.FillType 属性。此属性将在自 2016 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


表示指定填充的纹理类型。

参见 [TextureType](../../com.aspose.cells/texturetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


返回或设置区域的透明度，取值范围为 0.0（不透明）至 1.0（完全透明）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


将指定的填充设置为双色渐变。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| color2 | [Color](../../com.aspose.cells/color) | 双色渐变。 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


将指定的填充设置为双色渐变。仅适用于 Excel 2007。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | 单一渐变颜色。 |
| transparency1 | double | color1 的透明度程度，取值范围为 0.0（不透明）至 1.0（透明）。 |
| color2 | [Color](../../com.aspose.cells/color) | 双色渐变。 |
| transparency2 | double | color2 的透明度程度，取值范围为 0.0（不透明）至 1.0（透明）。 |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype)。渐变阴影样式。 |
| variant | int | 渐变的变体。取值范围为 1 到 4，对应“填充效果”对话框中“渐变”选项卡上的四种变体之一。如果样式为 GradientStyle.FromCenter，则 Variant 参数只能为 1 或 2。 |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


设置填充类型。

参见 [FillType](../../com.aspose.cells/filltype)。

**Remarks**

注意：此成员现已过时。请改用 FillFormat.FillType 属性。此属性将在自 2016 年 7 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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

