---
title: "Axis"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un asse di un grafico."
type: docs
url: /it/java/com.aspose.cells/axis/
---

**Inheritance:**
java.lang.Object
```
public class Axis
```

Incapsula l'oggetto che rappresenta un asse di un grafico.

**Example**

Dal codice seguente, puoi apprendere come impostare l'unità, il valore massimo e minimo dell'asse.

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
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(4);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(20);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 25, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
         chart.getNSeries().add("A1:B3", true);
         //Set the max value of value axis
         chart.getValueAxis().setMaxValue(200);
         //Set the min value of value axis
         chart.getValueAxis().setMinValue(0);
         //Set the major unit
         chart.getValueAxis().setMajorUnit(25);
         //Category(X) axis crosses at the maxinum value.
         chart.getValueAxis().setCrossType(CrossType.MAXIMUM);
         //Set he number of categories or series between tick-mark labels. 
         chart.getCategoryAxis().setTickLabelSpacing(2);
 
         //do your business
 
         //Saving the Excel file
         workbook.save("book1.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Ottiene il [getArea()](../../com.aspose.cells/axis\#getArea--). |
| [getAxisBetweenCategories()](#getAxisBetweenCategories--) | Rappresenta se l'asse dei valori attraversa l'asse delle categorie tra le categorie. |
| [getAxisLabels()](#getAxisLabels--) | Ottiene le etichette dell'asse dopo la chiamata al metodo Chart.Calculate(). |
| [getAxisLine()](#getAxisLine--) | Ottiene l'aspetto di un asse. |
| [getAxisTexts()](#getAxisTexts--) | Ottiene le etichette dell'asse dopo la chiamata al metodo Chart.Calculate(). |
| [getBaseUnitScale()](#getBaseUnitScale--) | Rappresenta la scala dell'unità base per l'asse delle categorie. |
| [getBins()](#getBins--) | Rappresenta i contenitori su un asse di grafico (Istogramma/Pareto) |
| [getCategoryType()](#getCategoryType--) | Rappresenta il tipo dell'asse delle categorie. |
| [getClass()](#getClass--) |  |
| [getCrossAt()](#getCrossAt--) | Rappresenta il punto sull'asse dei valori dove l'asse delle categorie lo attraversa. |
| [getCrossType()](#getCrossType--) | Rappresenta il [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sull'asse specificato dove l'altro asse lo attraversa. |
| [getCustUnit()](#getCustUnit--) | Specifica un valore personalizzato per l'unità di visualizzazione. |
| [getCustomDisplayUnit()](#getCustomDisplayUnit--) | Specifica un valore personalizzato per l'unità di visualizzazione. |
| [getCustomUnit()](#getCustomUnit--) | Specifica un valore personalizzato per l'unità di visualizzazione. |
| [getDisplayUnit()](#getDisplayUnit--) | Rappresenta l'etichetta dell'unità per l'asse specificato. |
| [getDisplayUnitLabel()](#getDisplayUnitLabel--) | Rappresenta un'etichetta di unità su un asse nel grafico specificato. |
| [getLogBase()](#getLogBase--) | Rappresenta la base logaritmica. |
| [getMajorGridLines()](#getMajorGridLines--) | Rappresenta le linee della griglia principali su un asse del grafico. |
| [getMajorTickMark()](#getMajorTickMark--) | Rappresenta il tipo di segno di spunta principale per l'asse specificato. |
| [getMajorUnit()](#getMajorUnit--) | Rappresenta le unità principali per l'asse. |
| [getMajorUnitScale()](#getMajorUnitScale--) | Rappresenta la scala dell'unità principale per l'asse di categoria. |
| [getMaxValue()](#getMaxValue--) | Rappresenta il valore massimo sull'asse dei valori. |
| [getMinValue()](#getMinValue--) | Rappresenta il valore minimo sull'asse dei valori. |
| [getMinorGridLines()](#getMinorGridLines--) | Rappresenta le linee della griglia secondarie su un asse del grafico. |
| [getMinorTickMark()](#getMinorTickMark--) | Rappresenta il tipo di segno di spunta secondario per l'asse specificato. |
| [getMinorUnit()](#getMinorUnit--) | Rappresenta le unità secondarie per l'asse. |
| [getMinorUnitScale()](#getMinorUnitScale--) | Rappresenta la scala dell'unità principale per l'asse di categoria. |
| [getTickLabelPosition()](#getTickLabelPosition--) | Rappresenta la posizione delle etichette dei segni di spunta sull'asse specificato. |
| [getTickLabelSpacing()](#getTickLabelSpacing--) | Rappresenta il numero di categorie o serie tra le etichette dei segni di spunta. |
| [getTickLabels()](#getTickLabels--) | Restituisce un oggetto [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) che rappresenta le etichette dei segni di spunta per l'asse specificato. |
| [getTickMarkSpacing()](#getTickMarkSpacing--) | Restituisce o imposta il numero di categorie o serie tra i segni di spunta. |
| [getTitle()](#getTitle--) | Recupera il titolo di questo asse nel grafico. |
| [hasMultiLevelLabels()](#hasMultiLevelLabels--) | Indica se le etichette devono essere visualizzate a più livelli. |
| [hashCode()](#hashCode--) |  |
| [isAutoTickLabelSpacing()](#isAutoTickLabelSpacing--) | Indica se la spaziatura delle etichette dei segni di spunta è automatica |
| [isAutomaticMajorUnit()](#isAutomaticMajorUnit--) | Indica se l'unità principale dell'asse è assegnata automaticamente. |
| [isAutomaticMaxValue()](#isAutomaticMaxValue--) | Indica se il valore massimo è assegnato automaticamente. |
| [isAutomaticMinValue()](#isAutomaticMinValue--) | Indica se il valore minimo è assegnato automaticamente. |
| [isAutomaticMinorUnit()](#isAutomaticMinorUnit--) | Indica se l'unità secondaria dell'asse è assegnata automaticamente. |
| [isBaseUnitAuto()](#isBaseUnitAuto--) | Rappresenta se l'unità di base è automatica. |
| [isDisplayUnitLabelShown()](#isDisplayUnitLabelShown--) | Rappresenta se l'etichetta dell'unità di visualizzazione è mostrata sull'asse specificato. |
| [isLogarithmic()](#isLogarithmic--) | Rappresenta se il tipo di scala dell'asse dei valori è logaritmico o meno. |
| [isPlotOrderReversed()](#isPlotOrderReversed--) | Rappresenta se Microsoft Excel traccia i punti dati dall'ultimo al primo. |
| [isVisible()](#isVisible--) | Rappresenta se l'asse è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoTickLabelSpacing(boolean value)](#setAutoTickLabelSpacing-boolean-) | Indica se la spaziatura delle etichette dei segni di spunta è automatica |
| [setAutomaticMajorUnit(boolean value)](#setAutomaticMajorUnit-boolean-) | Indica se l'unità principale dell'asse è assegnata automaticamente. |
| [setAutomaticMaxValue(boolean value)](#setAutomaticMaxValue-boolean-) | Indica se il valore massimo è assegnato automaticamente. |
| [setAutomaticMinValue(boolean value)](#setAutomaticMinValue-boolean-) | Indica se il valore minimo è assegnato automaticamente. |
| [setAutomaticMinorUnit(boolean value)](#setAutomaticMinorUnit-boolean-) | Indica se l'unità secondaria dell'asse è assegnata automaticamente. |
| [setAxisBetweenCategories(boolean value)](#setAxisBetweenCategories-boolean-) | Rappresenta se l'asse dei valori attraversa l'asse delle categorie tra le categorie. |
| [setBaseUnitAuto(boolean value)](#setBaseUnitAuto-boolean-) | Rappresenta se l'unità di base è automatica. |
| [setBaseUnitScale(int value)](#setBaseUnitScale-int-) | Rappresenta la scala dell'unità base per l'asse delle categorie. |
| [setCategoryType(int value)](#setCategoryType-int-) | Rappresenta il tipo dell'asse delle categorie. |
| [setCrossAt(double value)](#setCrossAt-double-) | Rappresenta il punto sull'asse dei valori dove l'asse delle categorie lo attraversa. |
| [setCrossType(int value)](#setCrossType-int-) | Rappresenta il [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sull'asse specificato dove l'altro asse lo attraversa. |
| [setCustUnit(int value)](#setCustUnit-int-) | Specifica un valore personalizzato per l'unità di visualizzazione. |
| [setCustomDisplayUnit(double value)](#setCustomDisplayUnit-double-) | Specifica un valore personalizzato per l'unità di visualizzazione. |
| [setCustomUnit(int value)](#setCustomUnit-int-) | Specifica un valore personalizzato per l'unità di visualizzazione. |
| [setDisplayUnit(int value)](#setDisplayUnit-int-) | Rappresenta l'etichetta dell'unità per l'asse specificato. |
| [setDisplayUnitLabelShown(boolean value)](#setDisplayUnitLabelShown-boolean-) | Rappresenta se l'etichetta dell'unità di visualizzazione è mostrata sull'asse specificato. |
| [setHasMultiLevelLabels(boolean value)](#setHasMultiLevelLabels-boolean-) | Indica se le etichette devono essere visualizzate a più livelli. |
| [setLogBase(double value)](#setLogBase-double-) | Rappresenta la base logaritmica. |
| [setLogarithmic(boolean value)](#setLogarithmic-boolean-) | Rappresenta se il tipo di scala dell'asse dei valori è logaritmico o meno. |
| [setMajorTickMark(int value)](#setMajorTickMark-int-) | Rappresenta il tipo di segno di spunta principale per l'asse specificato. |
| [setMajorUnit(double value)](#setMajorUnit-double-) | Rappresenta le unità principali per l'asse. |
| [setMajorUnitScale(int value)](#setMajorUnitScale-int-) | Rappresenta la scala dell'unità principale per l'asse di categoria. |
| [setMaxValue(Object value)](#setMaxValue-java.lang.Object-) | Rappresenta il valore massimo sull'asse dei valori. |
| [setMinValue(Object value)](#setMinValue-java.lang.Object-) | Rappresenta il valore minimo sull'asse dei valori. |
| [setMinorTickMark(int value)](#setMinorTickMark-int-) | Rappresenta il tipo di segno di spunta secondario per l'asse specificato. |
| [setMinorUnit(double value)](#setMinorUnit-double-) | Rappresenta le unità secondarie per l'asse. |
| [setMinorUnitScale(int value)](#setMinorUnitScale-int-) | Rappresenta la scala dell'unità principale per l'asse di categoria. |
| [setPlotOrderReversed(boolean value)](#setPlotOrderReversed-boolean-) | Rappresenta se Microsoft Excel traccia i punti dati dall'ultimo al primo. |
| [setTickLabelPosition(int value)](#setTickLabelPosition-int-) | Rappresenta la posizione delle etichette dei segni di spunta sull'asse specificato. |
| [setTickLabelSpacing(int value)](#setTickLabelSpacing-int-) | Rappresenta il numero di categorie o serie tra le etichette dei segni di spunta. |
| [setTickMarkSpacing(int value)](#setTickMarkSpacing-int-) | Restituisce o imposta il numero di categorie o serie tra i segni di spunta. |
| [setVisible(boolean value)](#setVisible-boolean-) | Rappresenta se l'asse è visibile. |
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
### getArea() {#getArea--}
```
public Area getArea()
```


Ottiene il [getArea()](../../com.aspose.cells/axis\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAxisBetweenCategories() {#getAxisBetweenCategories--}
```
public boolean getAxisBetweenCategories()
```


Rappresenta se l'asse dei valori attraversa l'asse delle categorie tra le categorie.

**Remarks**

Questa proprietà si applica solo agli assi di categoria e non si applica ai grafici 3-D.

**Returns:**
boolean
### getAxisLabels() {#getAxisLabels--}
```
public ArrayList getAxisLabels()
```


Ottiene le etichette dell'asse dopo la chiamata al metodo Chart.Calculate().

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Axis.GetAxisTexts. Questa proprietà sarà rimossa tra 12 mesi a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
java.util.ArrayList
### getAxisLine() {#getAxisLine--}
```
public Line getAxisLine()
```


Ottiene l'aspetto di un asse.

**Returns:**
[Line](../../com.aspose.cells/line)
### getAxisTexts() {#getAxisTexts--}
```
public String[] getAxisTexts()
```


Ottiene le etichette dell'asse dopo la chiamata al metodo Chart.Calculate().

**Returns:**
java.lang.String[]
### getBaseUnitScale() {#getBaseUnitScale--}
```
public int getBaseUnitScale()
```


Rappresenta la scala dell'unità base per l'asse delle categorie.

Vedi [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Ha effetto solo quando la proprietà CategoryType è impostata su TimeScale.

**Returns:**
int
### getBins() {#getBins--}
```
public AxisBins getBins()
```


Rappresenta i contenitori su un asse di grafico (Istogramma/Pareto)

**Remarks**

Solo per grafico Histogram o Pareto.

**Returns:**
[AxisBins](../../com.aspose.cells/axisbins)
### getCategoryType() {#getCategoryType--}
```
public int getCategoryType()
```


Rappresenta il tipo dell'asse delle categorie.

Vedi [CategoryType](../../com.aspose.cells/categorytype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCrossAt() {#getCrossAt--}
```
public double getCrossAt()
```


Rappresenta il punto sull'asse dei valori dove l'asse delle categorie lo attraversa.

**Remarks**

Il numero deve essere un intero quando si applica all'asse di categoria. Inoltre il valore deve essere compreso tra 1 e 31999.

**Returns:**
double
### getCrossType() {#getCrossType--}
```
public int getCrossType()
```


Rappresenta il [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sull'asse specificato dove l'altro asse lo attraversa.

Vedi [CrossType](../../com.aspose.cells/crosstype).

**Returns:**
int
### getCustUnit() {#getCustUnit--}
```
public int getCustUnit()
```


Specifica un valore personalizzato per l'unità di visualizzazione.

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà Axis.CustomUnit. Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
int
### getCustomDisplayUnit() {#getCustomDisplayUnit--}
```
public double getCustomDisplayUnit()
```


Specifica un valore personalizzato per l'unità di visualizzazione.

**Returns:**
double
### getCustomUnit() {#getCustomUnit--}
```
public int getCustomUnit()
```


Specifica un valore personalizzato per l'unità di visualizzazione.

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà Axis.CustomDisplayUnit. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
int
### getDisplayUnit() {#getDisplayUnit--}
```
public int getDisplayUnit()
```


Rappresenta l'etichetta dell'unità per l'asse specificato.

Vedi [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Returns:**
int
### getDisplayUnitLabel() {#getDisplayUnitLabel--}
```
public DisplayUnitLabel getDisplayUnitLabel()
```


Rappresenta un'etichetta di unità su un asse nel grafico specificato. Le etichette di unità sono utili per rappresentare valori grandi, ad esempio in milioni o miliardi.

**Returns:**
[DisplayUnitLabel](../../com.aspose.cells/displayunitlabel)
### getLogBase() {#getLogBase--}
```
public double getLogBase()
```


Rappresenta la base logaritmica. Il valore predefinito è 10.

**Returns:**
double
### getMajorGridLines() {#getMajorGridLines--}
```
public Line getMajorGridLines()
```


Rappresenta le linee della griglia principali su un asse del grafico.

**Example**

```
         chart.getValueAxis().getMajorGridLines().setVisible(false);
         chart.getCategoryAxis().getMajorGridLines().setVisible(true);
```

**Returns:**
[Line](../../com.aspose.cells/line)
### getMajorTickMark() {#getMajorTickMark--}
```
public int getMajorTickMark()
```


Rappresenta il tipo di segno di spunta principale per l'asse specificato.

Vedi [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMajorUnit() {#getMajorUnit--}
```
public double getMajorUnit()
```


Rappresenta le unità principali per l'asse.

**Remarks**

Le unità principali devono essere maggiori di zero.

**Returns:**
double
### getMajorUnitScale() {#getMajorUnitScale--}
```
public int getMajorUnitScale()
```


Rappresenta la scala dell'unità principale per l'asse di categoria.

Vedi [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         /*TimeUnit*/int majorUnitScale = chart.getCategoryAxis().getMajorUnitScale(); //get
         chart.getCategoryAxis().setMajorUnitScale(majorUnitScale); //set
         chart.getCategoryAxis().setMajorUnit(2);
```

**Returns:**
int
### getMaxValue() {#getMaxValue--}
```
public Object getMaxValue()
```


Rappresenta il valore massimo sull'asse dei valori.

**Remarks**

Il tipo maxValue può essere solo double o DateTime.

**Returns:**
java.lang.Object
### getMinValue() {#getMinValue--}
```
public Object getMinValue()
```


Rappresenta il valore minimo sull'asse dei valori.

**Remarks**

Il tipo minValue può essere solo double o DateTime.

**Returns:**
java.lang.Object
### getMinorGridLines() {#getMinorGridLines--}
```
public Line getMinorGridLines()
```


Rappresenta le linee della griglia secondarie su un asse del grafico.

**Returns:**
[Line](../../com.aspose.cells/line)
### getMinorTickMark() {#getMinorTickMark--}
```
public int getMinorTickMark()
```


Rappresenta il tipo di segno di spunta secondario per l'asse specificato.

Vedi [TickMarkType](../../com.aspose.cells/tickmarktype).

**Returns:**
int
### getMinorUnit() {#getMinorUnit--}
```
public double getMinorUnit()
```


Rappresenta le unità secondarie per l'asse.

**Remarks**

Le unità minori devono essere maggiori di zero.

**Returns:**
double
### getMinorUnitScale() {#getMinorUnitScale--}
```
public int getMinorUnitScale()
```


Rappresenta la scala dell'unità principale per l'asse di categoria.

Vedi [TimeUnit](../../com.aspose.cells/timeunit).

**Example**

```
         chart.getCategoryAxis().setCategoryType(CategoryType.TIME_SCALE);
         chart.getCategoryAxis().setMinorUnitScale(TimeUnit.MONTHS);
         chart.getCategoryAxis().setMinorUnit(2);
```

**Returns:**
int
### getTickLabelPosition() {#getTickLabelPosition--}
```
public int getTickLabelPosition()
```


Rappresenta la posizione delle etichette dei segni di spunta sull'asse specificato.

Vedi [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Returns:**
int
### getTickLabelSpacing() {#getTickLabelSpacing--}
```
public int getTickLabelSpacing()
```


Rappresenta il numero di categorie o serie tra le etichette dei segni di graduazione. Si applica solo agli assi di categoria e di serie.

**Remarks**

Il numero deve essere compreso tra 1 e 31999.

**Returns:**
int
### getTickLabels() {#getTickLabels--}
```
public TickLabels getTickLabels()
```


Restituisce un oggetto [getTickLabels()](../../com.aspose.cells/axis\#getTickLabels--) che rappresenta le etichette dei segni di spunta per l'asse specificato.

**Returns:**
[TickLabels](../../com.aspose.cells/ticklabels)
### getTickMarkSpacing() {#getTickMarkSpacing--}
```
public int getTickMarkSpacing()
```


Restituisce o imposta il numero di categorie o serie tra i segni di graduazione. Si applica solo agli assi di categoria e di serie.

**Remarks**

Il numero deve essere compreso tra 1 e 31999.

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Recupera il titolo di questo asse nel grafico.

**Returns:**
[Title](../../com.aspose.cells/title)
### hasMultiLevelLabels() {#hasMultiLevelLabels--}
```
public boolean hasMultiLevelLabels()
```


Indica se le etichette devono essere visualizzate a più livelli.

**Remarks**

Valido solo per l'asse di categoria.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoTickLabelSpacing() {#isAutoTickLabelSpacing--}
```
public boolean isAutoTickLabelSpacing()
```


Indica se la spaziatura delle etichette dei segni di spunta è automatica

**Returns:**
boolean
### isAutomaticMajorUnit() {#isAutomaticMajorUnit--}
```
public boolean isAutomaticMajorUnit()
```


Indica se l'unità principale dell'asse è assegnata automaticamente.

**Returns:**
boolean
### isAutomaticMaxValue() {#isAutomaticMaxValue--}
```
public boolean isAutomaticMaxValue()
```


Indica se il valore massimo è assegnato automaticamente.

**Returns:**
boolean
### isAutomaticMinValue() {#isAutomaticMinValue--}
```
public boolean isAutomaticMinValue()
```


Indica se il valore minimo è assegnato automaticamente.

**Returns:**
boolean
### isAutomaticMinorUnit() {#isAutomaticMinorUnit--}
```
public boolean isAutomaticMinorUnit()
```


Indica se l'unità secondaria dell'asse è assegnata automaticamente.

**Returns:**
boolean
### isBaseUnitAuto() {#isBaseUnitAuto--}
```
public boolean isBaseUnitAuto()
```


Rappresenta se l'unità di base è automatica.

**Returns:**
boolean
### isDisplayUnitLabelShown() {#isDisplayUnitLabelShown--}
```
public boolean isDisplayUnitLabelShown()
```


Rappresenta se l'etichetta dell'unità di visualizzazione è mostrata sull'asse specificato.

**Remarks**

Il valore predefinito è True. Funziona solo quando [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) non è [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Returns:**
boolean
### isLogarithmic() {#isLogarithmic--}
```
public boolean isLogarithmic()
```


Rappresenta se il tipo di scala dell'asse dei valori è logaritmico o meno.

**Returns:**
boolean
### isPlotOrderReversed() {#isPlotOrderReversed--}
```
public boolean isPlotOrderReversed()
```


Rappresenta se Microsoft Excel traccia i punti dati dall'ultimo al primo.

**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Rappresenta se l'asse è visibile.

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




### setAutoTickLabelSpacing(boolean value) {#setAutoTickLabelSpacing-boolean-}
```
public void setAutoTickLabelSpacing(boolean value)
```


Indica se la spaziatura delle etichette dei segni di spunta è automatica

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutomaticMajorUnit(boolean value) {#setAutomaticMajorUnit-boolean-}
```
public void setAutomaticMajorUnit(boolean value)
```


Indica se l'unità principale dell'asse è assegnata automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutomaticMaxValue(boolean value) {#setAutomaticMaxValue-boolean-}
```
public void setAutomaticMaxValue(boolean value)
```


Indica se il valore massimo è assegnato automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutomaticMinValue(boolean value) {#setAutomaticMinValue-boolean-}
```
public void setAutomaticMinValue(boolean value)
```


Indica se il valore minimo è assegnato automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutomaticMinorUnit(boolean value) {#setAutomaticMinorUnit-boolean-}
```
public void setAutomaticMinorUnit(boolean value)
```


Indica se l'unità secondaria dell'asse è assegnata automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAxisBetweenCategories(boolean value) {#setAxisBetweenCategories-boolean-}
```
public void setAxisBetweenCategories(boolean value)
```


Rappresenta se l'asse dei valori attraversa l'asse delle categorie tra le categorie.

**Remarks**

Questa proprietà si applica solo agli assi di categoria e non si applica ai grafici 3-D.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBaseUnitAuto(boolean value) {#setBaseUnitAuto-boolean-}
```
public void setBaseUnitAuto(boolean value)
```


Rappresenta se l'unità di base è automatica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBaseUnitScale(int value) {#setBaseUnitScale-int-}
```
public void setBaseUnitScale(int value)
```


Rappresenta la scala dell'unità base per l'asse delle categorie.

Vedi [TimeUnit](../../com.aspose.cells/timeunit).

**Remarks**

Ha effetto solo quando la proprietà CategoryType è impostata su TimeScale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCategoryType(int value) {#setCategoryType-int-}
```
public void setCategoryType(int value)
```


Rappresenta il tipo dell'asse delle categorie.

Vedi [CategoryType](../../com.aspose.cells/categorytype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCrossAt(double value) {#setCrossAt-double-}
```
public void setCrossAt(double value)
```


Rappresenta il punto sull'asse dei valori dove l'asse delle categorie lo attraversa.

**Remarks**

Il numero deve essere un intero quando si applica all'asse di categoria. Inoltre il valore deve essere compreso tra 1 e 31999.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setCrossType(int value) {#setCrossType-int-}
```
public void setCrossType(int value)
```


Rappresenta il [getCrossType()](../../com.aspose.cells/axis\#getCrossType--) sull'asse specificato dove l'altro asse lo attraversa.

Vedi [CrossType](../../com.aspose.cells/crosstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCustUnit(int value) {#setCustUnit-int-}
```
public void setCustUnit(int value)
```


Specifica un valore personalizzato per l'unità di visualizzazione.

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà Axis.CustomUnit. Questa proprietà sarà rimossa tra 12 mesi a partire da gennaio 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCustomDisplayUnit(double value) {#setCustomDisplayUnit-double-}
```
public void setCustomDisplayUnit(double value)
```


Specifica un valore personalizzato per l'unità di visualizzazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setCustomUnit(int value) {#setCustomUnit-int-}
```
public void setCustomUnit(int value)
```


Specifica un valore personalizzato per l'unità di visualizzazione.

**Remarks**

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà Axis.CustomDisplayUnit. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDisplayUnit(int value) {#setDisplayUnit-int-}
```
public void setDisplayUnit(int value)
```


Rappresenta l'etichetta dell'unità per l'asse specificato.

Vedi [DisplayUnitType](../../com.aspose.cells/displayunittype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDisplayUnitLabelShown(boolean value) {#setDisplayUnitLabelShown-boolean-}
```
public void setDisplayUnitLabelShown(boolean value)
```


Rappresenta se l'etichetta dell'unità di visualizzazione è mostrata sull'asse specificato.

**Remarks**

Il valore predefinito è True. Funziona solo quando [getDisplayUnit()](../../com.aspose.cells/axis\#getDisplayUnit--) non è [DisplayUnitType.NONE](../../com.aspose.cells/displayunittype\#NONE).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHasMultiLevelLabels(boolean value) {#setHasMultiLevelLabels-boolean-}
```
public void setHasMultiLevelLabels(boolean value)
```


Indica se le etichette devono essere visualizzate a più livelli.

**Remarks**

Valido solo per l'asse di categoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLogBase(double value) {#setLogBase-double-}
```
public void setLogBase(double value)
```


Rappresenta la base logaritmica. Il valore predefinito è 10.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLogarithmic(boolean value) {#setLogarithmic-boolean-}
```
public void setLogarithmic(boolean value)
```


Rappresenta se il tipo di scala dell'asse dei valori è logaritmico o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMajorTickMark(int value) {#setMajorTickMark-int-}
```
public void setMajorTickMark(int value)
```


Rappresenta il tipo di segno di spunta principale per l'asse specificato.

Vedi [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMajorUnit(double value) {#setMajorUnit-double-}
```
public void setMajorUnit(double value)
```


Rappresenta le unità principali per l'asse.

**Remarks**

Le unità principali devono essere maggiori di zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setMajorUnitScale(int value) {#setMajorUnitScale-int-}
```
public void setMajorUnitScale(int value)
```


Rappresenta la scala dell'unità principale per l'asse di categoria.

Vedi [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMaxValue(Object value) {#setMaxValue-java.lang.Object-}
```
public void setMaxValue(Object value)
```


Rappresenta il valore massimo sull'asse dei valori.

**Remarks**

Il tipo maxValue può essere solo double o DateTime.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### setMinValue(Object value) {#setMinValue-java.lang.Object-}
```
public void setMinValue(Object value)
```


Rappresenta il valore minimo sull'asse dei valori.

**Remarks**

Il tipo minValue può essere solo double o DateTime.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### setMinorTickMark(int value) {#setMinorTickMark-int-}
```
public void setMinorTickMark(int value)
```


Rappresenta il tipo di segno di spunta secondario per l'asse specificato.

Vedi [TickMarkType](../../com.aspose.cells/tickmarktype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMinorUnit(double value) {#setMinorUnit-double-}
```
public void setMinorUnit(double value)
```


Rappresenta le unità secondarie per l'asse.

**Remarks**

Le unità minori devono essere maggiori di zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setMinorUnitScale(int value) {#setMinorUnitScale-int-}
```
public void setMinorUnitScale(int value)
```


Rappresenta la scala dell'unità principale per l'asse di categoria.

Vedi [TimeUnit](../../com.aspose.cells/timeunit).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPlotOrderReversed(boolean value) {#setPlotOrderReversed-boolean-}
```
public void setPlotOrderReversed(boolean value)
```


Rappresenta se Microsoft Excel traccia i punti dati dall'ultimo al primo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTickLabelPosition(int value) {#setTickLabelPosition-int-}
```
public void setTickLabelPosition(int value)
```


Rappresenta la posizione delle etichette dei segni di spunta sull'asse specificato.

Vedi [TickLabelPositionType](../../com.aspose.cells/ticklabelpositiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTickLabelSpacing(int value) {#setTickLabelSpacing-int-}
```
public void setTickLabelSpacing(int value)
```


Rappresenta il numero di categorie o serie tra le etichette dei segni di graduazione. Si applica solo agli assi di categoria e di serie.

**Remarks**

Il numero deve essere compreso tra 1 e 31999.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTickMarkSpacing(int value) {#setTickMarkSpacing-int-}
```
public void setTickMarkSpacing(int value)
```


Restituisce o imposta il numero di categorie o serie tra i segni di graduazione. Si applica solo agli assi di categoria e di serie.

**Remarks**

Il numero deve essere compreso tra 1 e 31999.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Rappresenta se l'asse è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

