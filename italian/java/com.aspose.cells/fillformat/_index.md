---
title: "FillFormat"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta la formattazione di riempimento per una forma."
type: docs
url: /it/java/com.aspose.cells/fillformat/
---

**Inheritance:**
java.lang.Object
```
public class FillFormat
```

Incapsula l'oggetto che rappresenta la formattazione di riempimento per una forma.

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
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | Ottiene il tipo di riempimento |
| [getGradientColor1()](#getGradientColor1--) | Restituisce il colore gradiente 1 per il riempimento specificato. |
| [getGradientColor2()](#getGradientColor2--) | Restituisce il colore gradiente 2 per il riempimento specificato. |
| [getGradientColorType()](#getGradientColorType--) | Restituisce il tipo di colore gradiente per il riempimento specificato. |
| [getGradientDegree()](#getGradientDegree--) | Restituisce il grado di gradiente per il riempimento specificato. |
| [getGradientFill()](#getGradientFill--) | Ottiene l'oggetto [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | Restituisce lo stile di gradiente per il riempimento specificato. |
| [getGradientVariant()](#getGradientVariant--) | Restituisce la variante di gradiente per il riempimento specificato. |
| [getImageData()](#getImageData--) | Ottiene i dati dell'immagine. |
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
| [hashCode()](#hashCode--) | Ottiene il codice hash. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | Imposta il tipo di riempimento |
| [setImageData(byte[] value)](#setImageData-byte---) | Imposta i dati dell'immagine. |
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
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
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
### hashCode() {#hashCode--}
```
public int hashCode()
```


Ottiene il codice hash.

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

