---
title: "FillFormat"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar fyllningsformatering för en form."
type: docs
url: /sv/java/com.aspose.cells/fillformat/
---

**Inheritance:**
java.lang.Object
```
public class FillFormat
```

Inkapslar objektet som representerar fyllningsformatering för en form.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | Hämtar fyllningstyp |
| [getGradientColor1()](#getGradientColor1--) | Returnerar gradientfärg 1 för den angivna fyllningen. |
| [getGradientColor2()](#getGradientColor2--) | Returnerar gradientfärg 2 för den angivna fyllningen. |
| [getGradientColorType()](#getGradientColorType--) | Returnerar gradientfärgens typ för den angivna fyllningen. |
| [getGradientDegree()](#getGradientDegree--) | Returnerar gradientens grad för den angivna fyllningen. |
| [getGradientFill()](#getGradientFill--) | Hämtar [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) objektet. |
| [getGradientStyle()](#getGradientStyle--) | Returnerar gradientstilen för den angivna fyllningen. |
| [getGradientVariant()](#getGradientVariant--) | Returnerar gradientvarianten för den angivna fyllningen. |
| [getImageData()](#getImageData--) | Hämtar bilddata. |
| [getPattern()](#getPattern--) | Representerar ett områdes visningsmönster. |
| [getPatternFill()](#getPatternFill--) | Hämtar [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) objektet. |
| [getPictureFormatType()](#getPictureFormatType--) | Hämtar bildformatets typ. |
| [getPresetColor()](#getPresetColor--) | Returnerar gradientens förinställda färg för den angivna fyllningen. |
| [getScale()](#getScale--) | Hämtar bildformatets skala. |
| [getSetType()](#getSetType--) | Hämtar fyllningsformatets typ. |
| [getSolidFill()](#getSolidFill--) | Hämtar [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) objektet. |
| [getTexture()](#getTexture--) | Representerar texturtypen för den angivna fyllningen. |
| [getTextureFill()](#getTextureFill--) | Hämtar [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) objektet. |
| [getTransparency()](#getTransparency--) | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |
| [getType()](#getType--) | Hämtar fyllningstypen. |
| [hashCode()](#hashCode--) | Hämtar hashkoden. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | Ställer in fyllningstypen |
| [setImageData(byte[] value)](#setImageData-byte---) | Ställer in bilddata. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Anger den angivna fyllningen till en enfärgsgradient. |
| [setPattern(int value)](#setPattern-int-) | Representerar ett områdes visningsmönster. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Ställer in bildformatstypen. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Ställer in den angivna fyllningen till en förinställd färggradient. |
| [setScale(double value)](#setScale-double-) | Ställer in bildformatskalan. |
| [setSetType(int value)](#setSetType-int-) | Hämtar fyllningsformatets typ. |
| [setTexture(int value)](#setTexture-int-) | Representerar texturtypen för den angivna fyllningen. |
| [setTransparency(double value)](#setTransparency-double-) | Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Ställer in den angivna fyllningen till en tvåfärgsgradient. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Ställer in den angivna fyllningen till en tvåfärgsgradient. |
| [setType(int value)](#setType-int-) | Ställer in fyllningstypen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Hämtar fyllningstyp

Se [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Returnerar gradientfärg 1 för den angivna fyllningen.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Returnerar gradientfärg 2 för den angivna fyllningen.

**Remarks**

Endast när gradientfärgens typ är GradientColorType.TwoColors är denna egenskap meningsfull.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Returnerar gradientfärgens typ för den angivna fyllningen.

Se [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Returnerar gradientens grad för den angivna fyllningen. Gäller endast för Excel 2007.

**Remarks**

Kan endast vara ett värde mellan 0,0 (mörk) och 1,0 (ljus).

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Hämtar [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) objektet.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Returnerar gradientstilen för den angivna fyllningen.

Se [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Returnerar gradientvarianten för den angivna fyllningen. Gäller endast för Excel 2007.

**Remarks**

Kan endast vara ett värde mellan 1 och 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fylleeffekter. Om stil är GradientStyle.FromCenter kan Variant‑argumentet endast vara 1 eller 2.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Hämtar bilddata.

**Remarks**

Om fyllningsformatet inte är ett anpassat texturformat returneras null.

**Returns:**
byte[]
### getPattern() {#getPattern--}
```
public int getPattern()
```


Representerar ett områdes visningsmönster.

Se [FillPattern](../../com.aspose.cells/fillpattern).

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Hämtar [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) objektet.

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Hämtar bildformatets typ.

Se [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Returnerar gradientens förinställda färg för den angivna fyllningen.

Se [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Hämtar bildformatets skala.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Hämtar fyllningsformatets typ.

Se [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället egenskapen FillFormat.FillType. Denna egenskap kommer att tas bort 12 månader senare, sedan juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Hämtar [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) objektet.

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Representerar texturtypen för den angivna fyllningen.

Se [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Hämtar [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) objektet.

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Hämtar fyllningstypen.

Se [FillType](../../com.aspose.cells/filltype).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället egenskapen FillFormat.FillType. Denna egenskap kommer att tas bort 12 månader senare, sedan juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Hämtar hashkoden.

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


Ställer in fyllningstypen

Se [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Ställer in bilddata.

**Remarks**

Om fyllningsformatet inte är ett anpassat texturformat returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| grad | double | Gradientgraden. Kan vara ett värde från 0.0 (mörk) till 1.0 (ljus). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Representerar ett områdes visningsmönster.

Se [FillPattern](../../com.aspose.cells/fillpattern).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Ställer in bildformatstypen.

Se [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Ställer in den angivna fyllningen till en förinställd färggradient. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Förinställd färgtyp |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Ställer in bildformatskalan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Hämtar fyllningsformatets typ.

Se [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället egenskapen FillFormat.FillType. Denna egenskap kommer att tas bort 12 månader senare, sedan juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Representerar texturtypen för den angivna fyllningen.

Se [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Returnerar eller anger graden av transparens för området som ett värde från 0,0 (opak) till 1,0 (klar).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| color2 | [Color](../../com.aspose.cells/color) | Två gradientfärger. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| transparency1 | double | Grad av transparens för färg1 som ett värde från 0,0 (opakt) till 1,0 (genomskinligt). |
| color2 | [Color](../../com.aspose.cells/color) | Två gradientfärger. |
| transparency2 | double | Grad av transparens för färg2 som ett värde från 0,0 (opakt) till 1,0 (genomskinligt). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Ställer in fyllningstypen.

Se [FillType](../../com.aspose.cells/filltype).

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället egenskapen FillFormat.FillType. Denna egenskap kommer att tas bort 12 månader senare, sedan juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

