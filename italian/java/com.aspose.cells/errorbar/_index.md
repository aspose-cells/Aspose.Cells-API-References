---
title: "ErrorBar"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la barra di errore della serie di dati."
type: docs
url: /it/java/com.aspose.cells/errorbar/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class ErrorBar extends Line
```

Rappresenta la barra di errore della serie di dati.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("a1").putValue(2);
         cells.get("a2").putValue(5);
         cells.get("a3").putValue(3);
         cells.get("a4").putValue(6);
         cells.get("b1").putValue(4);
         cells.get("b2").putValue(3);
         cells.get("b3").putValue(6);
         cells.get("b4").putValue(7);
 
         cells.get("C1").putValue("Q1");
         cells.get("C2").putValue("Q2");
         cells.get("C3").putValue("Y1");
         cells.get("C4").putValue("Y2");
 
         int chartIndex = workbook.getWorksheets().get(0).getCharts().add(ChartType.COLUMN, 11, 0, 27, 10);
 
         Chart chart = workbook.getWorksheets().get(0).getCharts().get(chartIndex);
         chart.getNSeries().add("A1:B4", true);
 
         chart.getNSeries().setCategoryData("C1:C4");
 
         for(int i = 0; i <chart.getNSeries().getCount(); i ++)
         {
         		Series aseries = chart.getNSeries().get(i);
         		aseries.getYErrorBar().setDisplayType(ErrorBarDisplayType.MINUS);
         		aseries.getYErrorBar().setType(ErrorBarType.FIXED_VALUE);
         		aseries.getYErrorBar().setAmount(5);
         }
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAmount()](#getAmount--) | Rappresenta la quantità di barra di errore. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Specifica la lunghezza della punta della freccia per l'inizio di una linea. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [getBeginType()](#getBeginType--) | Specifica una punta di freccia per l'inizio di una linea. |
| [getCapType()](#getCapType--) | Specifica i cappucci finali. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Rappresenta il [Color](../../com.aspose.cells/color) della linea. |
| [getCompoundType()](#getCompoundType--) | Specifica il tipo di linea composto |
| [getDashType()](#getDashType--) | Specifica il tipo di linea tratteggiata |
| [getDisplayType()](#getDisplayType--) | Rappresenta il tipo di visualizzazione della barra di errore. |
| [getEndArrowLength()](#getEndArrowLength--) | Specifica la lunghezza della punta della freccia per l'estremità di una linea. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Specifica la larghezza della punta della freccia per l'estremità di una linea. |
| [getEndType()](#getEndType--) | Specifica una punta di freccia per l'estremità di una linea. |
| [getFormattingType()](#getFormattingType--) | Ottiene il tipo di formato. |
| [getGradientFill()](#getGradientFill--) | Rappresenta il riempimento gradiente. |
| [getJoinType()](#getJoinType--) | Specifica i cappucci di giunzione. |
| [getMinusValue()](#getMinusValue--) | Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato. |
| [getPlusValue()](#getPlusValue--) | Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato. |
| [getShowMarkerTTop()](#getShowMarkerTTop--) | Indica se formattare le barre di errore con un T-top. |
| [getStyle()](#getStyle--) | Rappresenta lo stile della linea. |
| [getThemeColor()](#getThemeColor--) | Ottiene il colore del tema. |
| [getTransparency()](#getTransparency--) | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [getType()](#getType--) | Rappresenta il tipo di quantità della barra di errore. |
| [getWeight()](#getWeight--) | Ottiene il [WeightType](../../com.aspose.cells/weighttype) della linea. |
| [getWeightPt()](#getWeightPt--) | Ottiene il peso della linea in unità di punti. |
| [getWeightPx()](#getWeightPx--) | Ottiene il peso della linea in unità di pixel. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indica se questo stile di linea è assegnato automaticamente. |
| [isAutomaticColor()](#isAutomaticColor--) | Indica se il colore della linea è assegnato automaticamente. |
| [isVisible()](#isVisible--) | Rappresenta se la linea è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAmount(double value)](#setAmount-double-) | Rappresenta la quantità di barra di errore. |
| [setAuto(boolean value)](#setAuto-boolean-) | Indica se questo stile di linea è assegnato automaticamente. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Specifica la lunghezza della punta della freccia per l'inizio di una linea. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [setBeginType(int value)](#setBeginType-int-) | Specifica una punta di freccia per l'inizio di una linea. |
| [setCapType(int value)](#setCapType-int-) | Specifica i cappucci finali. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Rappresenta il [Color](../../com.aspose.cells/color) della linea. |
| [setCompoundType(int value)](#setCompoundType-int-) | Specifica il tipo di linea composto |
| [setDashType(int value)](#setDashType-int-) | Specifica il tipo di linea tratteggiata |
| [setDisplayType(int value)](#setDisplayType-int-) | Rappresenta il tipo di visualizzazione della barra di errore. |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Specifica la lunghezza della punta della freccia per l'estremità di una linea. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Specifica la larghezza della punta della freccia per l'estremità di una linea. |
| [setEndType(int value)](#setEndType-int-) | Specifica una punta di freccia per l'estremità di una linea. |
| [setFormattingType(int value)](#setFormattingType-int-) | Imposta il tipo di formato. |
| [setJoinType(int value)](#setJoinType-int-) | Specifica i cappucci di giunzione. |
| [setMinusValue(String value)](#setMinusValue-java.lang.String-) | Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato. |
| [setPlusValue(String value)](#setPlusValue-java.lang.String-) | Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato. |
| [setShowMarkerTTop(boolean value)](#setShowMarkerTTop-boolean-) | Indica se formattare le barre di errore con un T-top. |
| [setStyle(int value)](#setStyle-int-) | Rappresenta lo stile della linea. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Imposta il colore del tema. |
| [setTransparency(double value)](#setTransparency-double-) | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [setType(int value)](#setType-int-) | Rappresenta il tipo di quantità della barra di errore. |
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
### getAmount() {#getAmount--}
```
public double getAmount()
```


Rappresenta la quantità di barra di errore.

**Remarks**

La quantità deve essere maggiore o uguale a zero.

**Returns:**
double
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
### getDisplayType() {#getDisplayType--}
```
public int getDisplayType()
```


Rappresenta il tipo di visualizzazione della barra di errore.

See [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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
### getMinusValue() {#getMinusValue--}
```
public String getMinusValue()
```


Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato.

**Returns:**
java.lang.String
### getPlusValue() {#getPlusValue--}
```
public String getPlusValue()
```


Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato.

**Returns:**
java.lang.String
### getShowMarkerTTop() {#getShowMarkerTTop--}
```
public boolean getShowMarkerTTop()
```


Indica se formattare le barre di errore con un T-top.

**Returns:**
boolean
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
### getType() {#getType--}
```
public int getType()
```


Rappresenta il tipo di quantità della barra di errore.

See [ErrorBarType](../../com.aspose.cells/errorbartype).

**Example**

```
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         Series aseries = chart.getNSeries().get(0);
         //Gets custom error bar type
         /*ErrorBarType*/int errBarType = aseries.getYErrorBar().getType();
         //Sets custom error bar type
         aseries.getYErrorBar().setType(ErrorBarType.CUSTOM);
         aseries.getYErrorBar().setPlusValue("=Sheet1!A1");
         aseries.getYErrorBar().setMinusValue("=Sheet1!A2");
```

**Returns:**
int
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




### setAmount(double value) {#setAmount-double-}
```
public void setAmount(double value)
```


Rappresenta la quantità di barra di errore.

**Remarks**

La quantità deve essere maggiore o uguale a zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

### setDisplayType(int value) {#setDisplayType-int-}
```
public void setDisplayType(int value)
```


Rappresenta il tipo di visualizzazione della barra di errore.

See [ErrorBarDisplayType](../../com.aspose.cells/errorbardisplaytype).

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

### setMinusValue(String value) {#setMinusValue-java.lang.String-}
```
public void setMinusValue(String value)
```


Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setPlusValue(String value) {#setPlusValue-java.lang.String-}
```
public void setPlusValue(String value)
```


Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setShowMarkerTTop(boolean value) {#setShowMarkerTTop-boolean-}
```
public void setShowMarkerTTop(boolean value)
```


Indica se formattare le barre di errore con un T-top.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Rappresenta il tipo di quantità della barra di errore.

See [ErrorBarType](../../com.aspose.cells/errorbartype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

