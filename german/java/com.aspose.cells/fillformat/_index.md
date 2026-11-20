---
title: "FillFormat"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das die Füllformatierung für eine Form darstellt."
type: docs
url: /de/java/com.aspose.cells/fillformat/
---

**Inheritance:**
java.lang.Object
```
public class FillFormat
```

Kapselt das Objekt, das die Füllformatierung für eine Form darstellt.

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | Ruft den Fülltyp ab. |
| [getGradientColor1()](#getGradientColor1--) | Gibt die Farbverlauffarbe 1 für die angegebene Füllung zurück. |
| [getGradientColor2()](#getGradientColor2--) | Gibt die Farbverlauffarbe 2 für die angegebene Füllung zurück. |
| [getGradientColorType()](#getGradientColorType--) | Gibt den Farbverlauf-Farbtyp für die angegebene Füllung zurück. |
| [getGradientDegree()](#getGradientDegree--) | Gibt den Grad des Farbverlaufs für die angegebene Füllung zurück. |
| [getGradientFill()](#getGradientFill--) | Ruft das Objekt [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) ab. |
| [getGradientStyle()](#getGradientStyle--) | Gibt den Stil des Farbverlaufs für die angegebene Füllung zurück. |
| [getGradientVariant()](#getGradientVariant--) | Gibt die Variante des Farbverlaufs für die angegebene Füllung zurück. |
| [getImageData()](#getImageData--) | Ruft die Bilddaten des Bildes ab. |
| [getPattern()](#getPattern--) | Stellt ein Anzeigemuster eines Bereichs dar. |
| [getPatternFill()](#getPatternFill--) | Ruft das Objekt [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) ab. |
| [getPictureFormatType()](#getPictureFormatType--) | Ermittelt den Bildformattyp. |
| [getPresetColor()](#getPresetColor--) | Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück. |
| [getScale()](#getScale--) | Ermittelt die Bildformatskalierung. |
| [getSetType()](#getSetType--) | Ruft den festgelegten Füllformattyp ab. |
| [getSolidFill()](#getSolidFill--) | Ruft das Objekt [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) ab. |
| [getTexture()](#getTexture--) | Stellt den Texturtyp für die angegebene Füllung dar. |
| [getTextureFill()](#getTextureFill--) | Ruft das Objekt [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) ab. |
| [getTransparency()](#getTransparency--) | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [getType()](#getType--) | Ruft den Fülltyp ab. |
| [hashCode()](#hashCode--) | Ermittelt den Hashcode. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | Setzt den Fülltyp |
| [setImageData(byte[] value)](#setImageData-byte---) | Setzt die Bilddaten des Bildes. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf. |
| [setPattern(int value)](#setPattern-int-) | Stellt ein Anzeigemuster eines Bereichs dar. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Legt den Bildformattyp fest. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. |
| [setScale(double value)](#setScale-double-) | Legt die Bildformat-Skalierung fest. |
| [setSetType(int value)](#setSetType-int-) | Ruft den festgelegten Füllformattyp ab. |
| [setTexture(int value)](#setTexture-int-) | Stellt den Texturtyp für die angegebene Füllung dar. |
| [setTransparency(double value)](#setTransparency-double-) | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. |
| [setType(int value)](#setType-int-) | Setzt den Fülltyp. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
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


Ruft den Fülltyp ab.

Siehe [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Gibt die Farbverlauffarbe 1 für die angegebene Füllung zurück.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Gibt die Farbverlauffarbe 2 für die angegebene Füllung zurück.

**Remarks**

Nur wenn der Farbverlauf-Farbtyp GradientColorType.TwoColors ist, ist diese Eigenschaft sinnvoll.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Gibt den Farbverlauf-Farbtyp für die angegebene Füllung zurück.

Siehe [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Gibt den Gradientengrad für die angegebene Füllung zurück. Gilt nur für Excel 2007.

**Remarks**

Kann nur ein Wert von 0.0 (dunkel) bis 1.0 (hell) sein.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Ruft das Objekt [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) ab.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Gibt den Stil des Farbverlaufs für die angegebene Füllung zurück.

Siehe [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Gibt die Gradientvariante für die angegebene Füllung zurück. Gilt nur für Excel 2007.

**Remarks**

Kann nur ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Ruft die Bilddaten des Bildes ab.

**Remarks**

Wenn das Füllformat kein benutzerdefiniertes Texturformat ist, wird null zurückgegeben.

**Returns:**
byte[]
### getPattern() {#getPattern--}
```
public int getPattern()
```


Stellt ein Anzeigemuster eines Bereichs dar.

Siehe [FillPattern](../../com.aspose.cells/fillpattern).

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Ruft das Objekt [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--) ab.

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Ermittelt den Bildformattyp.

Siehe [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück.

Siehe [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Ermittelt die Bildformatskalierung.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Ruft den festgelegten Füllformattyp ab.

Siehe [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft FillFormat.FillType. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Ruft das Objekt [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--) ab.

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Stellt den Texturtyp für die angegebene Füllung dar.

Siehe [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Ruft das Objekt [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--) ab.

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Ruft den Fülltyp ab.

Siehe [FillType](../../com.aspose.cells/filltype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft FillFormat.FillType. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Ermittelt den Hashcode.

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


Setzt den Fülltyp

Siehe [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Setzt die Bilddaten des Bildes.

**Remarks**

Wenn das Füllformat kein benutzerdefiniertes Texturformat ist, wird null zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Setzt die angegebene Füllung auf einen Einfarbverlauf. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| Grad | double | Der Grad des Farbverlaufs. Kann ein Wert von 0.0 (dunkel) bis 1.0 (hell) sein. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Stellt ein Anzeigemuster eines Bereichs dar.

Siehe [FillPattern](../../com.aspose.cells/fillpattern).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Legt den Bildformattyp fest.

Siehe [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Vorgabefarbtyp |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Legt die Bildformat-Skalierung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Ruft den festgelegten Füllformattyp ab.

Siehe [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft FillFormat.FillType. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Stellt den Texturtyp für die angegebene Füllung dar.

Siehe [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| color2 | [Color](../../com.aspose.cells/color) | Zwei Gradientfarben. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| transparency1 | double | Der Transparenzgrad von color1 als Wert von 0.0 (undurchsichtig) bis 1.0 (klar). |
| color2 | [Color](../../com.aspose.cells/color) | Zwei Gradientfarben. |
| transparency2 | double | Der Transparenzgrad von color2 als Wert von 0.0 (undurchsichtig) bis 1.0 (klar). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Setzt den Fülltyp.

Siehe [FillType](../../com.aspose.cells/filltype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft FillFormat.FillType. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

