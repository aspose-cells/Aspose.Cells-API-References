---
title: "LineFormat"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta tutte le impostazioni della linea."
type: docs
url: /it/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

Rappresenta tutte le impostazioni della linea.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se questa istanza ha lo stesso valore di un altro oggetto [LineFormat](../../com.aspose.cells/lineformat) specificato. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | Restituisce il tipo di lunghezza della freccia iniziale della linea. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | Restituisce il tipo di freccia iniziale della linea. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | Restituisce il tipo di larghezza della freccia iniziale della linea. |
| [getCapType()](#getCapType--) | Specifica i cappucci finali. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | Specifica il tipo di composto della linea. |
| [getDashStyle()](#getDashStyle--) | Specifica il tipo di tratteggio della linea. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | Restituisce il tipo di lunghezza della freccia finale della linea. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | Restituisce il tipo di freccia finale della linea. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | Restituisce il tipo di larghezza della freccia finale della linea. |
| [getFillType()](#getFillType--) | Ottiene il tipo di riempimento |
| [getGradientColor1()](#getGradientColor1--) | Restituisce il colore gradiente 1 per il riempimento specificato. |
| [getGradientColor2()](#getGradientColor2--) | Restituisce il colore gradiente 2 per il riempimento specificato. |
| [getGradientColorType()](#getGradientColorType--) | Restituisce il tipo di colore gradiente per il riempimento specificato. |
| [getGradientDegree()](#getGradientDegree--) | Restituisce il grado di gradiente per il riempimento specificato. |
| [getGradientFill()](#getGradientFill--) | Ottiene l'oggetto [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | Restituisce lo stile di gradiente per il riempimento specificato. |
| [getGradientVariant()](#getGradientVariant--) | Restituisce la variante di gradiente per il riempimento specificato. |
| [getImageData()](#getImageData--) | Ottiene i dati dell'immagine. |
| [getJoinType()](#getJoinType--) | Specifica il tipo di giunzione della linea. |
| [getPattern()](#getPattern--) | Rappresenta il modello di visualizzazione di un'area. |
| [getPatternFill()](#getPatternFill--) | Ottiene l'oggetto [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--). |
| [getPictureFormatType()](#getPictureFormatType--) | Ottiene il tipo di formato immagine. |
| [getPresetColor()](#getPresetColor--) | Restituisce il colore predefinito del gradiente per il riempimento specificato. |
| [getScale()](#getScale--) | Ottiene la scala del formato immagine. |
| [getSetType()](#getSetType--) | Ottiene il tipo di set del formato di riempimento. |
| [getSolidFill()](#getSolidFill--) | Ottiene l'oggetto [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--). |
| [getTexture()](#getTexture--) | Rappresenta il tipo di texture per il riempimento specificato. |
| [getTextureFill()](#getTextureFill--) | Ottiene l'oggetto [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--). |
| [getTransparency()](#getTransparency--) | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [getType()](#getType--) | Ottiene il tipo di riempimento. |
| [getWeight()](#getWeight--) | Ottiene il peso della linea in unità di punti. |
| [hashCode()](#hashCode--) | Ottiene il codice hash. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | Imposta il tipo di lunghezza della freccia iniziale della linea. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | Imposta il tipo di freccia iniziale della linea. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | Imposta il tipo di larghezza della freccia iniziale della linea. |
| [setCapType(int value)](#setCapType-int-) | Specifica i cappucci finali. |
| [setCompoundType(int value)](#setCompoundType-int-) | Specifica il tipo di composto della linea. |
| [setDashStyle(int value)](#setDashStyle-int-) | Specifica il tipo di tratteggio della linea. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | Imposta il tipo di lunghezza della freccia finale della linea. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | Imposta il tipo di freccia finale della linea. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | Imposta il tipo di larghezza della freccia finale della linea. |
| [setFillType(int value)](#setFillType-int-) | Imposta il tipo di riempimento |
| [setImageData(byte[] value)](#setImageData-byte---) | Imposta i dati dell'immagine. |
| [setJoinType(int value)](#setJoinType-int-) | Specifica il tipo di giunzione della linea. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Imposta il riempimento specificato a un gradiente a un colore. |
| [setPattern(int value)](#setPattern-int-) | Rappresenta il modello di visualizzazione di un'area. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | Imposta il tipo di formato immagine. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Imposta il riempimento specificato a una sfumatura di colore predefinito. |
| [setScale(double value)](#setScale-double-) | Imposta la scala del formato immagine. |
| [setSetType(int value)](#setSetType-int-) | Ottiene il tipo di set del formato di riempimento. |
| [setTexture(int value)](#setTexture-int-) | Rappresenta il tipo di texture per il riempimento specificato. |
| [setTransparency(double value)](#setTransparency-double-) | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Imposta il riempimento specificato a un gradiente a due colori. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Imposta il riempimento specificato a un gradiente a due colori. |
| [setType(int value)](#setType-int-) | Imposta il tipo di riempimento. |
| [setWeight(double value)](#setWeight-double-) | Imposta il peso della linea in unità di punti. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina se questa istanza ha lo stesso valore di un altro oggetto [LineFormat](../../com.aspose.cells/lineformat) specificato.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto [LineFormat](../../com.aspose.cells/lineformat) da confrontare con questa istanza. |

**Returns:**
boolean - true se il valore del parametro obj è lo stesso del valore di questa istanza; altrimenti, false. Se obj è null, questo metodo restituisce false.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


Restituisce il tipo di lunghezza della freccia iniziale della linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Restituisce il tipo di freccia iniziale della linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Restituisce il tipo di larghezza della freccia iniziale della linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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


Specifica i cappucci finali.

Vedi [LineCapType](../../com.aspose.cells/linecaptype).

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


Specifica il tipo di composto della linea.

Vedi [MsoLineStyle](../../com.aspose.cells/msolinestyle).

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


Specifica il tipo di tratteggio della linea.

Vedi [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

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


Restituisce il tipo di lunghezza della freccia finale della linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

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


Restituisce il tipo di freccia finale della linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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


Restituisce il tipo di larghezza della freccia finale della linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

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


Ottiene il tipo di riempimento

Vedi [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Restituisce il colore gradiente 1 per il riempimento specificato.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Restituisce il colore gradiente 2 per il riempimento specificato.

**Remarks**

Solo quando il tipo di colore del gradiente è GradientColorType.TwoColors, questa proprietà ha senso.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Restituisce il tipo di colore gradiente per il riempimento specificato.

Vedi [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Restituisce il grado del gradiente per il riempimento specificato. Valido solo per Excel 2007.

**Remarks**

Può essere solo un valore da 0,0 (scuro) a 1,0 (chiaro).

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Ottiene l'oggetto [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--).

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Restituisce lo stile di gradiente per il riempimento specificato.

Vedi [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


Restituisce la variante del gradiente per il riempimento specificato. Valido solo per Excel 2007.

**Remarks**

Può essere solo un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


Ottiene i dati dell'immagine.

**Remarks**

Se il formato di riempimento non è un formato di texture personalizzato, restituisce null.

**Returns:**
byte[]
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Specifica il tipo di giunzione della linea.

Vedi [LineJoinType](../../com.aspose.cells/linejointype).

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


Rappresenta il modello di visualizzazione di un'area.

Vedi [FillPattern](../../com.aspose.cells/fillpattern).

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


Ottiene l'oggetto [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--).

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


Ottiene il tipo di formato immagine.

Vedi [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Restituisce il colore predefinito del gradiente per il riempimento specificato.

Vedi [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


Ottiene la scala del formato immagine.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


Ottiene il tipo di set del formato di riempimento.

Vedi [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FillFormat.FillType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


Ottiene l'oggetto [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--).

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


Rappresenta il tipo di texture per il riempimento specificato.

Vedi [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


Ottiene l'oggetto [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--).

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di riempimento.

Vedi [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FillFormat.FillType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getWeight() {#getWeight--}
```
public double getWeight()
```


Ottiene il peso della linea in unità di punti.

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


Ottiene il codice hash.

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


Imposta il tipo di lunghezza della freccia iniziale della linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


Imposta il tipo di freccia iniziale della linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


Imposta il tipo di larghezza della freccia iniziale della linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


Specifica i cappucci finali.

Vedi [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Specifica il tipo di composto della linea.

Vedi [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


Specifica il tipo di tratteggio della linea.

Vedi [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


Imposta il tipo di lunghezza della freccia finale della linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


Imposta il tipo di freccia finale della linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


Imposta il tipo di larghezza della freccia finale della linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


Imposta il tipo di riempimento

Vedi [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


Imposta i dati dell'immagine.

**Remarks**

Se il formato di riempimento non è un formato di texture personalizzato, restituisce null.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Specifica il tipo di giunzione della linea.

Vedi [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Imposta il riempimento specificato a un gradiente a un colore. Valido solo per Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| grado | double | Il grado del gradiente. Può essere un valore da 0.0 (scuro) a 1.0 (chiaro). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Rappresenta il modello di visualizzazione di un'area.

Vedi [FillPattern](../../com.aspose.cells/fillpattern).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


Imposta il tipo di formato immagine.

Vedi [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Imposta il riempimento specificato a un gradiente di colore predefinito. Valido solo per Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Tipo di colore predefinito |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


Imposta la scala del formato immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


Ottiene il tipo di set del formato di riempimento.

Vedi [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FillFormat.FillType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


Rappresenta il tipo di texture per il riempimento specificato.

Vedi [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| color2 | [Color](../../com.aspose.cells/color) | Due colori del gradiente. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Imposta il riempimento specificato a un gradiente a due colori. Valido solo per Excel 2007.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| transparency1 | double | Il grado di trasparenza del colore1 come valore da 0,0 (opaco) a 1,0 (trasparente). |
| color2 | [Color](../../com.aspose.cells/color) | Due colori del gradiente. |
| transparency2 | double | Il grado di trasparenza del colore2 come valore da 0,0 (opaco) a 1,0 (trasparente). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Imposta il tipo di riempimento.

Vedi [FillType](../../com.aspose.cells/filltype).

**Remarks**

NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FillFormat.FillType. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


Imposta il peso della linea in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

