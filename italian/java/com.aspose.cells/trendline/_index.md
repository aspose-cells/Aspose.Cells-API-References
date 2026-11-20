---
title: "Trendline"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta una linea di tendenza in un grafico."
type: docs
url: /it/java/com.aspose.cells/trendline/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Line](../../com.aspose.cells/line)
```
public class Trendline extends Line
```

Rappresenta una linea di tendenza in un grafico.

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
         chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //adding a linear trendline
         int index = chart.getNSeries().get(0).getTrendLines().add(TrendlineType.LINEAR);
         Trendline trendline = chart.getNSeries().get(0).getTrendLines().get(index);
         //Setting the custom name of the trendline.
         trendline.setName("Linear");
         //Displaying the equation on chart
         trendline.setDisplayEquation(true);
         //Displaying the R-Squared value on chart
         trendline.setDisplayRSquared(true);
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackward()](#getBackward--) | Restituisce o imposta il numero di periodi (o unità in un grafico a dispersione) a cui la trendline si estende all'indietro. |
| [getBeginArrowLength()](#getBeginArrowLength--) | Specifica la lunghezza della punta della freccia per l'inizio di una linea. |
| [getBeginArrowWidth()](#getBeginArrowWidth--) | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [getBeginType()](#getBeginType--) | Specifica una punta di freccia per l'inizio di una linea. |
| [getCapType()](#getCapType--) | Specifica i cappucci finali. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Rappresenta il [Color](../../com.aspose.cells/color) della linea. |
| [getCompoundType()](#getCompoundType--) | Specifica il tipo di linea composto |
| [getDashType()](#getDashType--) | Specifica il tipo di linea tratteggiata |
| [getDataLabels()](#getDataLabels--) | Rappresenta l'oggetto DataLabels per la serie specificata. |
| [getDisplayEquation()](#getDisplayEquation--) | Rappresenta se l'equazione della linea di tendenza è visualizzata sul grafico (nella stessa etichetta dati del valore R-squared). |
| [getDisplayRSquared()](#getDisplayRSquared--) | Rappresenta se il valore R-squared della linea di tendenza è visualizzato sul grafico (nella stessa etichetta dati dell'equazione). |
| [getEndArrowLength()](#getEndArrowLength--) | Specifica la lunghezza della punta della freccia per l'estremità di una linea. |
| [getEndArrowWidth()](#getEndArrowWidth--) | Specifica la larghezza della punta della freccia per l'estremità di una linea. |
| [getEndType()](#getEndType--) | Specifica una punta di freccia per l'estremità di una linea. |
| [getFormattingType()](#getFormattingType--) | Ottiene il tipo di formato. |
| [getForward()](#getForward--) | Restituisce o imposta il numero di periodi (o unità in un grafico a dispersione) a cui la linea di tendenza si estende in avanti. |
| [getGradientFill()](#getGradientFill--) | Rappresenta il riempimento gradiente. |
| [getIntercept()](#getIntercept--) | Restituisce o imposta il punto in cui la linea di tendenza attraversa l'asse dei valori. |
| [getJoinType()](#getJoinType--) | Specifica i cappucci di giunzione. |
| [getLegendEntry()](#getLegendEntry--) | Ottiene la voce della legenda relativa a questa linea di tendenza |
| [getName()](#getName--) | Restituisce il nome della linea di tendenza. |
| [getOrder()](#getOrder--) | Restituisce o imposta l'ordine della linea di tendenza (un intero maggiore di 1) quando il tipo di linea di tendenza è Polinomiale. |
| [getPeriod()](#getPeriod--) | Restituisce o imposta il periodo per la linea di tendenza a media mobile. |
| [getStyle()](#getStyle--) | Rappresenta lo stile della linea. |
| [getThemeColor()](#getThemeColor--) | Ottiene il colore del tema. |
| [getTransparency()](#getTransparency--) | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente). |
| [getType()](#getType--) | Restituisce il tipo di linea di tendenza. |
| [getWeight()](#getWeight--) | Ottiene il [WeightType](../../com.aspose.cells/weighttype) della linea. |
| [getWeightPt()](#getWeightPt--) | Ottiene il peso della linea in unità di punti. |
| [getWeightPx()](#getWeightPx--) | Ottiene il peso della linea in unità di pixel. |
| [hashCode()](#hashCode--) |  |
| [isAuto()](#isAuto--) | Indica se questo stile di linea è assegnato automaticamente. |
| [isAutomaticColor()](#isAutomaticColor--) | Indica se il colore della linea è assegnato automaticamente. |
| [isInterceptAuto()](#isInterceptAuto--) | Indica se Microsoft Workbook determina automaticamente l'intercetta della linea di tendenza. |
| [isNameAuto()](#isNameAuto--) | Restituisce se Microsoft Excel determina automaticamente il nome della linea di tendenza. |
| [isVisible()](#isVisible--) | Rappresenta se la linea è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuto(boolean value)](#setAuto-boolean-) | Indica se questo stile di linea è assegnato automaticamente. |
| [setBackward(double value)](#setBackward-double-) | Restituisce o imposta il numero di periodi (o unità in un grafico a dispersione) a cui la trendline si estende all'indietro. |
| [setBeginArrowLength(int value)](#setBeginArrowLength-int-) | Specifica la lunghezza della punta della freccia per l'inizio di una linea. |
| [setBeginArrowWidth(int value)](#setBeginArrowWidth-int-) | Specifica la larghezza della punta della freccia per l'inizio di una linea. |
| [setBeginType(int value)](#setBeginType-int-) | Specifica una punta di freccia per l'inizio di una linea. |
| [setCapType(int value)](#setCapType-int-) | Specifica i cappucci finali. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Rappresenta il [Color](../../com.aspose.cells/color) della linea. |
| [setCompoundType(int value)](#setCompoundType-int-) | Specifica il tipo di linea composto |
| [setDashType(int value)](#setDashType-int-) | Specifica il tipo di linea tratteggiata |
| [setDisplayEquation(boolean value)](#setDisplayEquation-boolean-) | Rappresenta se l'equazione della linea di tendenza è visualizzata sul grafico (nella stessa etichetta dati del valore R-squared). |
| [setDisplayRSquared(boolean value)](#setDisplayRSquared-boolean-) | Rappresenta se il valore R-squared della linea di tendenza è visualizzato sul grafico (nella stessa etichetta dati dell'equazione). |
| [setEndArrowLength(int value)](#setEndArrowLength-int-) | Specifica la lunghezza della punta della freccia per l'estremità di una linea. |
| [setEndArrowWidth(int value)](#setEndArrowWidth-int-) | Specifica la larghezza della punta della freccia per l'estremità di una linea. |
| [setEndType(int value)](#setEndType-int-) | Specifica una punta di freccia per l'estremità di una linea. |
| [setFormattingType(int value)](#setFormattingType-int-) | Imposta il tipo di formato. |
| [setForward(double value)](#setForward-double-) | Restituisce o imposta il numero di periodi (o unità in un grafico a dispersione) a cui la linea di tendenza si estende in avanti. |
| [setIntercept(double value)](#setIntercept-double-) | Restituisce o imposta il punto in cui la linea di tendenza attraversa l'asse dei valori. |
| [setInterceptAuto(boolean isInterceptAuto)](#setInterceptAuto-boolean-) | Imposta se Microsoft Workbook determina automaticamente l'intercetta della linea di tendenza. |
| [setJoinType(int value)](#setJoinType-int-) | Specifica i cappucci di giunzione. |
| [setName(String value)](#setName-java.lang.String-) | Restituisce il nome della linea di tendenza. |
| [setNameAuto(boolean value)](#setNameAuto-boolean-) | Restituisce se Microsoft Excel determina automaticamente il nome della linea di tendenza. |
| [setOrder(int value)](#setOrder-int-) | Restituisce o imposta l'ordine della linea di tendenza (un intero maggiore di 1) quando il tipo di linea di tendenza è Polinomiale. |
| [setPeriod(int value)](#setPeriod-int-) | Restituisce o imposta il periodo per la linea di tendenza a media mobile. |
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
### getBackward() {#getBackward--}
```
public double getBackward()
```


Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) a cui la linea di tendenza si estende all'indietro. Il numero di periodi deve essere maggiore o uguale a zero. Se il tipo di grafico è colonna, il numero di periodi deve essere compreso tra 0 e 0,5.

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
### getDataLabels() {#getDataLabels--}
```
public DataLabels getDataLabels()
```


Rappresenta l'oggetto DataLabels per la serie specificata.

**Returns:**
[DataLabels](../../com.aspose.cells/datalabels)
### getDisplayEquation() {#getDisplayEquation--}
```
public boolean getDisplayEquation()
```


Rappresenta se l'equazione della linea di tendenza è visualizzata sul grafico (nella stessa etichetta dati del valore R-squared). Impostare questa proprietà su True attiva automaticamente le etichette dati.

**Returns:**
boolean
### getDisplayRSquared() {#getDisplayRSquared--}
```
public boolean getDisplayRSquared()
```


Rappresenta se il valore R-squared della linea di tendenza è visualizzato sul grafico (nella stessa etichetta dati dell'equazione). Impostare questa proprietà su True attiva automaticamente le etichette dati.

**Returns:**
boolean
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
### getForward() {#getForward--}
```
public double getForward()
```


Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) a cui la linea di tendenza si estende in avanti. Il numero di periodi deve essere maggiore o uguale a zero.

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


Rappresenta il riempimento gradiente.

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getIntercept() {#getIntercept--}
```
public double getIntercept()
```


Restituisce o imposta il punto in cui la linea di tendenza attraversa l'asse dei valori.

**Returns:**
double
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


Specifica i cappucci di giunzione.

Vedi [LineJoinType](../../com.aspose.cells/linejointype).

**Returns:**
int
### getLegendEntry() {#getLegendEntry--}
```
public LegendEntry getLegendEntry()
```


Ottiene la voce della legenda relativa a questa linea di tendenza

**Returns:**
[LegendEntry](../../com.aspose.cells/legendentry)
### getName() {#getName--}
```
public String getName()
```


Restituisce il nome della linea di tendenza.

**Returns:**
java.lang.String
### getOrder() {#getOrder--}
```
public int getOrder()
```


Restituisce o imposta l'ordine della linea di tendenza (un intero maggiore di 1) quando il tipo di linea di tendenza è Polinomiale. L'ordine deve essere compreso tra 2 e 6.

**Returns:**
int
### getPeriod() {#getPeriod--}
```
public int getPeriod()
```


Restituisce o imposta il periodo per la linea di tendenza a media mobile.

**Remarks**

Questo valore dovrebbe essere compreso tra 2 e 255. E deve essere inferiore al numero di punti del grafico nella serie

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
### getType() {#getType--}
```
public int getType()
```


Restituisce il tipo di linea di tendenza.

Vedi [TrendlineType](../../com.aspose.cells/trendlinetype).

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
### isInterceptAuto() {#isInterceptAuto--}
```
public boolean isInterceptAuto()
```


Indica se Microsoft Workbook determina automaticamente l'intercetta della linea di tendenza.

**Returns:**
boolean
### isNameAuto() {#isNameAuto--}
```
public boolean isNameAuto()
```


Restituisce se Microsoft Excel determina automaticamente il nome della linea di tendenza.

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

### setBackward(double value) {#setBackward-double-}
```
public void setBackward(double value)
```


Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) a cui la linea di tendenza si estende all'indietro. Il numero di periodi deve essere maggiore o uguale a zero. Se il tipo di grafico è colonna, il numero di periodi deve essere compreso tra 0 e 0,5.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

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

### setDisplayEquation(boolean value) {#setDisplayEquation-boolean-}
```
public void setDisplayEquation(boolean value)
```


Rappresenta se l'equazione della linea di tendenza è visualizzata sul grafico (nella stessa etichetta dati del valore R-squared). Impostare questa proprietà su True attiva automaticamente le etichette dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDisplayRSquared(boolean value) {#setDisplayRSquared-boolean-}
```
public void setDisplayRSquared(boolean value)
```


Rappresenta se il valore R-squared della linea di tendenza è visualizzato sul grafico (nella stessa etichetta dati dell'equazione). Impostare questa proprietà su True attiva automaticamente le etichette dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setForward(double value) {#setForward-double-}
```
public void setForward(double value)
```


Restituisce o imposta il numero di periodi (o unità su un grafico a dispersione) a cui la linea di tendenza si estende in avanti. Il numero di periodi deve essere maggiore o uguale a zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setIntercept(double value) {#setIntercept-double-}
```
public void setIntercept(double value)
```


Restituisce o imposta il punto in cui la linea di tendenza attraversa l'asse dei valori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setInterceptAuto(boolean isInterceptAuto) {#setInterceptAuto-boolean-}
```
public void setInterceptAuto(boolean isInterceptAuto)
```


Imposta se Microsoft Workbook determina automaticamente l'intercetta della linea di tendenza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isInterceptAuto | boolean |  |

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

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Restituisce il nome della linea di tendenza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNameAuto(boolean value) {#setNameAuto-boolean-}
```
public void setNameAuto(boolean value)
```


Restituisce se Microsoft Excel determina automaticamente il nome della linea di tendenza.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOrder(int value) {#setOrder-int-}
```
public void setOrder(int value)
```


Restituisce o imposta l'ordine della linea di tendenza (un intero maggiore di 1) quando il tipo di linea di tendenza è Polinomiale. L'ordine deve essere compreso tra 2 e 6.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPeriod(int value) {#setPeriod-int-}
```
public void setPeriod(int value)
```


Restituisce o imposta il periodo per la linea di tendenza a media mobile.

**Remarks**

Questo valore dovrebbe essere compreso tra 2 e 255. E deve essere inferiore al numero di punti del grafico nella serie

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

