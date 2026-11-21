---
title: "LineFormat"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla inställningar för linjen."
type: docs
url: /sv/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Representerar alla inställningar för linjen.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestämmer om detta objekt har samma värde som ett annat specificerat [LineFormat](../../com.aspose.cells/lineformat) objekt. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Hämtar startpilens längdtyp för linjen. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Hämtar startpilens typ för linjen. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Hämtar startpilens breddtyp för linjen. |
| [getCapType()](#getCapType--) | Anger avslutningskapparna. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Anger linjens sammansättningstyp. |
| [getDashStyle()](#getDashStyle--) | Anger linjens strecktyp. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Hämtar slutpilens längdtyp för linjen. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Hämtar slutpilens typ för linjen. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Hämtar slutpilens breddtyp för linjen. |
| [getFillType()](#getFillType--) | Hämtar fyllningstyp |
| [getGradientColor1()](#getGradientColor1--) | Returnerar gradientfärg 1 för den angivna fyllningen. |
| [getGradientColor2()](#getGradientColor2--) | Returnerar gradientfärg 2 för den angivna fyllningen. |
| [getGradientColorType()](#getGradientColorType--) | Returnerar gradientfärgens typ för den angivna fyllningen. |
| [getGradientDegree()](#getGradientDegree--) | Returnerar gradientens grad för den angivna fyllningen. |
| [getGradientFill()](#getGradientFill--) | Hämtar [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) objektet. |
| [getGradientStyle()](#getGradientStyle--) | Returnerar gradientstilen för den angivna fyllningen. |
| [getGradientVariant()](#getGradientVariant--) | Returnerar gradientvarianten för den angivna fyllningen. |
| [getImageData()](#getImageData--) | Hämtar bilddata. |
| [getJoinType()](#getJoinType--) | Anger linjens sammanfogningstyp. |
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
| [getWeight()](#getWeight--) | Hämtar linjens vikt i enheter av punkter. |
| [hashCode()](#hashCode--) | Hämtar hashkoden. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Ställer in startpilens längdtyp för linjen. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Ställer in startpilens typ för linjen. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Ställer in startpilens breddtyp för linjen. |
| [setCapType(int value)](#setCapType-int-) | Anger avslutningskapparna. |
| [setCompoundType(int value)](#setCompoundType-int-) | Anger linjens sammansättningstyp. |
| [setDashStyle(int value)](#setDashStyle-int-) | Anger linjens strecktyp. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Ställer in slutpilens längdtyp för linjen. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Ställer in slutpilens typ för linjen. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Ställer in slutpilens breddtyp för linjen. |
| [setFillType(int value)](#setFillType-int-) | Ställer in fyllningstypen |
| [setImageData(byte[] value)](#setImageData-byte---) | Ställer in bilddata. |
| [setJoinType(int value)](#setJoinType-int-) | Anger linjens sammanfogningstyp. |
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
| [setWeight(double value)](#setWeight-double-) | Anger linjens vikt i enheter av punkter. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestämmer om detta objekt har samma värde som ett annat specificerat [LineFormat](../../com.aspose.cells/lineformat) objekt.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Det [LineFormat](../../com.aspose.cells/lineformat) objektet att jämföra med detta objekt. |

**Returns:**
boolean - sant om värdet på parametern obj är samma som värdet på detta objekt; annars falskt. Om obj är null returnerar denna metod falskt.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Hämtar startpilens längdtyp för linjen.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Hämtar startpilens typ för linjen.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Hämtar startpilens breddtyp för linjen.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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


Anger avslutningskapparna.

Se [LineCapType](../../com.aspose.cells/linecaptype).

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


Anger linjens sammansättningstyp.

Se [MsoLineStyle](../../com.aspose.cells/msolinestyle).

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


Anger linjens strecktyp.

Se [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

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


Hämtar slutpilens längdtyp för linjen.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Hämtar slutpilens typ för linjen.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Hämtar slutpilens breddtyp för linjen.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Anger linjens sammanfogningstyp.

Se [LineJoinType](../../com.aspose.cells/linejointype).

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
### getWeight() {#getWeight--}
```
public double getWeight()
```


Hämtar linjens vikt i enheter av punkter.

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


Hämtar hashkoden.

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


Ställer in startpilens längdtyp för linjen.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


Ställer in startpilens typ för linjen.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


Ställer in startpilens breddtyp för linjen.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Anger avslutningskapparna.

Se [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Anger linjens sammansättningstyp.

Se [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


Anger linjens strecktyp.

Se [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


Ställer in slutpilens längdtyp för linjen.

Se [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


Ställer in slutpilens typ för linjen.

Se [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


Ställer in slutpilens breddtyp för linjen.

Se [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Anger linjens sammanfogningstyp.

Se [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


Anger linjens vikt i enheter av punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

