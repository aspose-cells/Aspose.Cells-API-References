---
title: "Line"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta il formato della linea."
type: docs
url: /it/java/com.aspose.cells/line/
---

**Inheritance:**
java.lang.Object
```
public class Line
```

Incapsula l'oggetto che rappresenta il formato della linea.

**Example**

```
         Workbook workbook = new Workbook();
         	Worksheet sheet = workbook.getWorksheets().get(0);
 
         	Cells cells = sheet.getCells();
         	cells.get(0,1).putValue("Income");
         	cells.get(1,0).putValue("Company A");
         	cells.get(2,0).putValue("Company B");
         	cells.get(3,0).putValue("Company C");
         	cells.get(1,1).putValue(10000);
         	cells.get(2,1).putValue(20000);
         	cells.get(3,1).putValue(30000);
 
         	int chartIndex = sheet.getCharts().add(ChartType.LINE, 9, 9, 21, 15);
         Chart chart = sheet.getCharts().get(chartIndex);
         //Add series
         chart.getNSeries().add("A2:B4", true);
         //Set category data
         chart.getNSeries().setCategoryData("=Sheet1!$A$2:$A$4");
         //Applying a dotted line style on the lines of an NSeries
         chart.getNSeries().get(0).getBorder().setStyle(LineType.DOT);
         chart.getNSeries().get(0).getBorder().setColor(Color.getRed());
         //Applying a triangular marker style on the data markers of an NSeries
         chart.getNSeries().get(0).getMarker().setMarkerStyle(ChartMarkerType.TRIANGLE);
         //Setting the weight of all lines in an NSeries to medium
         chart.getNSeries().get(0).getBorder().setWeight(WeightType.MEDIUM_LINE);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBeginArrowLength()](#getBeginArrowLength--) | Specifica la lunghezza della punta della freccia per l'inizio di una linea. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [getBeginType()](#getBeginType--) | Specifica una punta di freccia per l'inizio di una linea. |
| [getCapType()](#getCapType--) | Specifica i cappucci finali. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Rappresenta il [Color](../../com.aspose.cells/color) della linea. |
| [getCompoundType()](#getCompoundType--) | Specifica il tipo di linea composto |
| [getDashType()](#getDashType--) | Specifica il tipo di linea tratteggiata |
| [getEndArrowLength()](#getEndArrowLength--) | Specifica la lunghezza della punta della freccia per l'estremità di una linea. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Specifica la larghezza della punta della freccia per l'estremità di una linea. |
| [getEndType()](#getEndType--) | Specifica una punta di freccia per l'estremità di una linea. |
| [getFormattingType()](#getFormattingType--) | Ottiene il tipo di formato. |
| [getGradientFill()](#getGradientFill--) | Rappresenta il riempimento gradiente. |
| [getJoinType()](#getJoinType--) | Specifica i cappucci di giunzione. |
| [getStyle()](#getStyle--) | Rappresenta lo stile della linea. |
| [getThemeColor()](#getThemeColor--) | Ottiene il colore del tema. |
| [getTransparency()](#getTransparency--) | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [getWeight()](#getWeight--) | Ottiene il [WeightType](../../com.aspose.cells/weighttype) della linea. |
| [getWeightPt()](#getWeightPt--) | Ottiene il peso della linea in unità di punti. |
| [getWeightPx()](#getWeightPx--) | Ottiene il peso della linea in unità di pixel. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indica se questo stile di linea è assegnato automaticamente. |
| [isAutomaticColor()](#isAutomaticColor--) | Indica se il colore della linea è assegnato automaticamente. |
| [isVisible()](#isVisible--) | Rappresenta se la linea è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indica se questo stile di linea è assegnato automaticamente. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Specifica la lunghezza della punta della freccia per l'inizio di una linea. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [setBeginType(int value)](#setBeginType-int-) | Specifica una punta di freccia per l'inizio di una linea. |
| [setCapType(int value)](#setCapType-int-) | Specifica i cappucci finali. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Rappresenta il [Color](../../com.aspose.cells/color) della linea. |
| [setCompoundType(int value)](#setCompoundType-int-) | Specifica il tipo di linea composto |
| [setDashType(int value)](#setDashType-int-) | Specifica il tipo di linea tratteggiata |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Specifica la lunghezza della punta della freccia per l'estremità di una linea. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Specifica la larghezza della punta della freccia per l'estremità di una linea. |
| [setEndType(int value)](#setEndType-int-) | Specifica una punta di freccia per l'estremità di una linea. |
| [setFormattingType(int value)](#setFormattingType-int-) | Imposta il tipo di formato. |
| [setJoinType(int value)](#setJoinType-int-) | Specifica i cappucci di giunzione. |
| [setStyle(int value)](#setStyle-int-) | Rappresenta lo stile della linea. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Imposta il colore del tema. |
| [setTransparency(double value)](#setTransparency-double-) | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [setVisible(boolean value)](#setVisible-boolean-) | Rappresenta se la linea è visibile. |
| [setWeight(int value)](#setWeight-int-) | Imposta il [WeightType](../../com.aspose.cells/weighttype) della linea. |
| [setWeightPt(double value)](#setWeightPt-double-) | Imposta il peso della linea in unità di punti. |
| [setWeightPx(double value)](#setWeightPx-double-) | Imposta il peso della linea in unità di pixel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBeginArrowLength() {#getBeginArrowLength--}
```
public int getBeginArrowLength()
```


Specifica la lunghezza della punta della freccia per l'inizio di una linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getBeginArrowWidth() {#getBeginArrowWidth--}
```
public int getBeginArrowWidth()
```


Specifica la larghezza della punta della freccia per l'inizio di una linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getBeginType() {#getBeginType--}
```
public int getBeginType()
```


Specifica una punta di freccia per l'inizio di una linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


Specifica i cappucci finali.

Vedi [LineCapType](../../com.aspose.cells/linecaptype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Rappresenta il [Color](../../com.aspose.cells/color) della linea.

**Returns:**
[Color](../../com.aspose.cells/color)
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


Specifica il tipo di linea composto

Vedi [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Returns:**
int
### getDashType() {#getDashType--}
```
public int getDashType()
```


Specifica il tipo di linea tratteggiata

Vedi [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Returns:**
int
### getEndArrowLength() {#getEndArrowLength--}
```
public int getEndArrowLength()
```


Specifica la lunghezza della punta della freccia per l'estremità di una linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Returns:**
int
### getEndArrowWidth() {#getEndArrowWidth--}
```
public int getEndArrowWidth()
```


Specifica la larghezza della punta della freccia per l'estremità di una linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Returns:**
int
### getEndType() {#getEndType--}
```
public int getEndType()
```


Specifica una punta di freccia per l'estremità di una linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Returns:**
int
### getFormattingType() {#getFormattingType--}
```
public int getFormattingType()
```


Ottiene il tipo di formato.

Vedi [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Returns:**
int
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Rappresenta il riempimento gradiente.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Specifica i cappucci di giunzione.

Vedi [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getStyle() {#getStyle--}
```
public int getStyle()
```


Rappresenta lo stile della linea.

Vedi [LineType](../../com.aspose.cells/linetype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Ottiene il colore del tema.

**Remarks**

Se il colore di primo piano non è un colore di tema, NULL verrà restituito.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente).

**Returns:**
double
### getWeight() {#getWeight--}
```
public int getWeight()
```


Ottiene il [WeightType](../../com.aspose.cells/weighttype) della linea.

Vedi [WeightType](../../com.aspose.cells/weighttype).

**Returns:**
int
### getWeightPt() {#getWeightPt--}
```
public double getWeightPt()
```


Ottiene il peso della linea in unità di punti.

**Returns:**
double
### getWeightPx() {#getWeightPx--}
```
public double getWeightPx()
```


Ottiene il peso della linea in unità di pixel.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAuto() {#isAuto--}
```
public boolean isAuto()
```


Indica se questo stile di linea è assegnato automaticamente.

**Returns:**
boolean
### isAutomaticColor() {#isAutomaticColor--}
```
public boolean isAutomaticColor()
```


Indica se il colore della linea è assegnato automaticamente.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Rappresenta se la linea è visibile.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAuto(boolean value) {#setAuto-boolean-}
```
public void setAuto(boolean value)
```


Indica se questo stile di linea è assegnato automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBeginArrowLength(int value) {#setBeginArrowLength-int-}
```
public void setBeginArrowLength(int value)
```


Specifica la lunghezza della punta della freccia per l'inizio di una linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBeginArrowWidth(int value) {#setBeginArrowWidth-int-}
```
public void setBeginArrowWidth(int value)
```


Specifica la larghezza della punta della freccia per l'inizio di una linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBeginType(int value) {#setBeginType-int-}
```
public void setBeginType(int value)
```


Specifica una punta di freccia per l'inizio di una linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

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

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Rappresenta il [Color](../../com.aspose.cells/color) della linea.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


Specifica il tipo di linea composto

Vedi [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDashType(int value) {#setDashType-int-}
```
public void setDashType(int value)
```


Specifica il tipo di linea tratteggiata

Vedi [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEndArrowLength(int value) {#setEndArrowLength-int-}
```
public void setEndArrowLength(int value)
```


Specifica la lunghezza della punta della freccia per l'estremità di una linea.

Vedi [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEndArrowWidth(int value) {#setEndArrowWidth-int-}
```
public void setEndArrowWidth(int value)
```


Specifica la larghezza della punta della freccia per l'estremità di una linea.

Vedi [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setEndType(int value) {#setEndType-int-}
```
public void setEndType(int value)
```


Specifica una punta di freccia per l'estremità di una linea.

Vedi [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFormattingType(int value) {#setFormattingType-int-}
```
public void setFormattingType(int value)
```


Imposta il tipo di formato.

Vedi [ChartLineFormattingType](../../com.aspose.cells/chartlineformattingtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


Specifica i cappucci di giunzione.

Vedi [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStyle(int value) {#setStyle-int-}
```
public void setStyle(int value)
```


Rappresenta lo stile della linea.

Vedi [LineType](../../com.aspose.cells/linetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Imposta il colore del tema.

**Remarks**

Se il colore di primo piano non è un colore di tema, NULL verrà restituito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Rappresenta se la linea è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWeight(int value) {#setWeight-int-}
```
public void setWeight(int value)
```


Imposta il [WeightType](../../com.aspose.cells/weighttype) della linea.

Vedi [WeightType](../../com.aspose.cells/weighttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWeightPt(double value) {#setWeightPt-double-}
```
public void setWeightPt(double value)
```


Imposta il peso della linea in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setWeightPx(double value) {#setWeightPx-double-}
```
public void setWeightPx(double value)
```


Imposta il peso della linea in unità di pixel.

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

