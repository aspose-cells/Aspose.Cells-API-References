---
title: "LineFormat"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle Einstellungen der Linie dar."
type: docs
url: /de/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Stellt alle Einstellungen der Linie dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes [LineFormat](../../com.aspose.cells/lineformat)-Objekt hat. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Ermittelt den Typ der Anfangspfeillänge der Linie. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Ermittelt den Typ des Anfangspfeils der Linie. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Ermittelt den Typ der Anfangspfeilbreite der Linie. |
| [getCapType()](#getCapType--) | Gibt die Endkappen an. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Gibt den zusammengesetzten Linientyp an. |
| [getDashStyle()](#getDashStyle--) | Gibt den Linienstiltyp an. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Ermittelt den Typ der Endpfeillänge der Linie. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Ermittelt den Typ des Endpfeils der Linie. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Ermittelt den Typ der Endpfeilbreite der Linie. |
| [getFillType()](#getFillType--) | Ruft den Fülltyp ab. |
| [getGradientColor1()](#getGradientColor1--) | Gibt die Farbverlauffarbe 1 für die angegebene Füllung zurück. |
| [getGradientColor2()](#getGradientColor2--) | Gibt die Farbverlauffarbe 2 für die angegebene Füllung zurück. |
| [getGradientColorType()](#getGradientColorType--) | Gibt den Farbverlauf-Farbtyp für die angegebene Füllung zurück. |
| [getGradientDegree()](#getGradientDegree--) | Gibt den Grad des Farbverlaufs für die angegebene Füllung zurück. |
| [getGradientFill()](#getGradientFill--) | Ruft das Objekt [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--) ab. |
| [getGradientStyle()](#getGradientStyle--) | Gibt den Stil des Farbverlaufs für die angegebene Füllung zurück. |
| [getGradientVariant()](#getGradientVariant--) | Gibt die Variante des Farbverlaufs für die angegebene Füllung zurück. |
| [getImageData()](#getImageData--) | Ruft die Bilddaten des Bildes ab. |
| [getJoinType()](#getJoinType--) | Gibt den Linienstückverbindungstyp an. |
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
| [getWeight()](#getWeight--) | Ermittelt das Gewicht der Linie in Punkten. |
| [hashCode()](#hashCode--) | Ermittelt den Hashcode. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Setzt den Typ der Anfangspfeillänge der Linie. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Setzt den Typ des Anfangspfeils der Linie. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Legt den Typ der Anfangspfeilbreite der Linie fest. |
| [setCapType(int value)](#setCapType-int-) | Gibt die Endkappen an. |
| [setCompoundType(int value)](#setCompoundType-int-) | Gibt den zusammengesetzten Linientyp an. |
| [setDashStyle(int value)](#setDashStyle-int-) | Gibt den Linienstiltyp an. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Legt den Typ der Endpfeillänge der Linie fest. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Legt den Typ des Endpfeils der Linie fest. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Legt den Typ der Endpfeilbreite der Linie fest. |
| [setFillType(int value)](#setFillType-int-) | Setzt den Fülltyp |
| [setImageData(byte[] value)](#setImageData-byte---) | Setzt die Bilddaten des Bildes. |
| [setJoinType(int value)](#setJoinType-int-) | Gibt den Linienstückverbindungstyp an. |
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
| [setWeight(double value)](#setWeight-double-) | Legt das Gewicht der Linie in Punkten fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestimmt, ob diese Instanz denselben Wert wie ein anderes angegebenes [LineFormat](../../com.aspose.cells/lineformat)-Objekt hat.

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das [LineFormat](../../com.aspose.cells/lineformat)-Objekt zum Vergleich mit dieser Instanz. |

**Returns:**
boolean - true, wenn der Wert des Parameters obj derselbe ist wie der Wert dieser Instanz; andernfalls false. Wenn obj null ist, gibt diese Methode false zurück.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Ermittelt den Typ der Anfangspfeillänge der Linie.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Ermittelt den Typ des Anfangspfeils der Linie.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Ermittelt den Typ der Anfangspfeilbreite der Linie.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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


Gibt die Endkappen an.

Siehe [LineCapType](../../com.aspose.cells/linecaptype).

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


Gibt den zusammengesetzten Linientyp an.

Siehe [MsoLineStyle](../../com.aspose.cells/msolinestyle).

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


Gibt den Linienstiltyp an.

Siehe [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

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


Ermittelt den Typ der Endpfeillänge der Linie.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Ermittelt den Typ des Endpfeils der Linie.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Ermittelt den Typ der Endpfeilbreite der Linie.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Gibt den Linienstückverbindungstyp an.

Siehe [LineJoinType](../../com.aspose.cells/linejointype).

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
### getWeight() {#getWeight--}
```
public double getWeight()
```


Ermittelt das Gewicht der Linie in Punkten.

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


Ermittelt den Hashcode.

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


Setzt den Typ der Anfangspfeillänge der Linie.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


Setzt den Typ des Anfangspfeils der Linie.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


Legt den Typ der Anfangspfeilbreite der Linie fest.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Gibt die Endkappen an.

Siehe [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Gibt den zusammengesetzten Linientyp an.

Siehe [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


Gibt den Linienstiltyp an.

Siehe [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


Legt den Typ der Endpfeillänge der Linie fest.

Siehe [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


Legt den Typ des Endpfeils der Linie fest.

Siehe [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


Legt den Typ der Endpfeilbreite der Linie fest.

Siehe [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Gibt den Linienstückverbindungstyp an.

Siehe [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


Legt das Gewicht der Linie in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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

