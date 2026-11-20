---
title: "DataLabels"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di tutti gli oggetti DataLabel per la Serie specificata."
type: docs
url: /it/java/com.aspose.cells/datalabels/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class DataLabels extends ChartTextFrame
```

Incapsula una raccolta di tutti gli oggetti DataLabel per la Serie specificata.

**Example**

```
         //Set the DataLabels in the chart
         Workbook wb = new Workbook("chart.xlsx");
         Chart chart = wb.getWorksheets().get(0).getCharts().get(0);
         DataLabels datalabels;
         for (int i = 0; i  <chart.getNSeries().getCount(); i++)
         {
             datalabels = chart.getNSeries().get(i).getDataLabels();
             //Set the position of DataLabels
             datalabels.setPosition(LabelPositionType.INSIDE_BASE);
             //Show the category name in the DataLabels
             datalabels.setShowCategoryName(true);
             //Show the value in the DataLabels
             datalabels.setShowValue(true);
             //Not show the percentage in the DataLabels
             datalabels.setShowPercentage(false);
             //Not show the legend key.
             datalabels.setShowLegendKey(false);
         }
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [applyFont()](#applyFont--) | Applica il carattere delle etichette dati a tutti i nodi figlio. |
| [characters(int startIndex, int length)](#characters-int-int-) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Ottiene il [getArea()](../../com.aspose.cells/datalabels\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [getBackground()](#getBackground--) | Ottiene la modalità di visualizzazione dello sfondo. |
| [getBackgroundMode()](#getBackgroundMode--) | Restituisce la modalità di visualizzazione dello sfondo |
| [getBorder()](#getBorder--) | Ottiene il [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Ottiene il grafico a cui appartiene questo oggetto. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Rappresenta l'altezza della posizione predefinita in unità di 1/4000 dell'area del grafico. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Rappresenta l'altezza della posizione predefinita in unità della frazione dell'area del grafico. |
| [getDefaultWidth()](#getDefaultWidth--) | Rappresenta la larghezza della posizione predefinita in unità di 1/4000 dell'area del grafico. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Rappresenta la larghezza della posizione predefinita in unità di frazione dell'area del grafico. |
| [getDefaultX()](#getDefaultX--) | Rappresenta x della posizione predefinita in unità di 1/4000 dell'area del grafico. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Rappresenta x della posizione predefinita in unità di frazione dell'area del grafico. |
| [getDefaultY()](#getDefaultY--) | Rappresenta y della posizione predefinita in unità di 1/4000 dell'area del grafico. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Rappresenta y della posizione predefinita in unità della frazione dell'area del grafico. |
| [getDirectionType()](#getDirectionType--) | Ottiene la direzione del testo. |
| [getFont()](#getFont--) | Ottiene il carattere delle DataLabels; |
| [getHeight()](#getHeight--) | Ottiene l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| [getHeightPixel()](#getHeightPixel--) | Ottiene l'altezza del frame in unità di pixel. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Ottiene l'altezza del frame in unità del rapporto dell'area del grafico. |
| [getLinkedSource()](#getLinkedSource--) | Ottiene un riferimento al foglio di lavoro. |
| [getNumber()](#getNumber--) | Ottiene il formato numerico incorporato. |
| [getNumberFormat()](#getNumberFormat--) | Rappresenta la stringa di formato per l'oggetto DataLabels. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | Vero se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle). |
| [getPosition()](#getPosition--) | Rappresenta la posizione dell'etichetta dati. |
| [getReadingOrder()](#getReadingOrder--) | Rappresenta l'ordine di lettura del testo. |
| [getRotationAngle()](#getRotationAngle--) | Rappresenta l'angolo di rotazione del testo. |
| [getSeparatorType()](#getSeparatorType--) | Ottiene il tipo di separatore usato per le etichette dati in un grafico. |
| [getSeparatorValue()](#getSeparatorValue--) | Ottiene il valore del separatore usato per le etichette dati in un grafico. |
| [getShadow()](#getShadow--) | Vero se il frame ha un'ombra. |
| [getShapeProperties()](#getShapeProperties--) | Ottiene l'oggetto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getShapeType()](#getShapeType--) | Ottiene il tipo di forma dell'etichetta dati. |
| [getShowBubbleSize()](#getShowBubbleSize--) | Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. |
| [getShowCategoryName()](#getShowCategoryName--) | Rappresenta il comportamento di visualizzazione del nome della categoria dell'etichetta dati di un grafico specificato. Vero per visualizzare il nome della categoria per le etichette dati in un grafico. |
| [getShowCellRange()](#getShowCellRange--) | Indica se mostrare l'intervallo di celle come etichette dati. |
| [getShowLegendKey()](#getShowLegendKey--) | Rappresenta il comportamento di visualizzazione della chiave della legenda dell'etichetta dati di un grafico specificato. |
| [getShowPercentage()](#getShowPercentage--) | Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. |
| [getShowSeriesName()](#getShowSeriesName--) | Indica se il nome della serie viene visualizzato sulle etichette dati in un grafico. |
| [getShowValue()](#getShowValue--) | Rappresenta il comportamento di visualizzazione dei valori dell'etichetta dati di un grafico specificato. |
| [getText()](#getText--) | Ottiene il testo dell'etichetta dati. |
| [getTextDirection()](#getTextDirection--) | Rappresenta l'ordine di lettura del testo. |
| [getTextFont()](#getTextFont--) | Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Ottiene l'allineamento orizzontale del testo. |
| [getTextOptions()](#getTextOptions--) | Ottiene le opzioni del testo. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Ottiene l'allineamento verticale del testo. |
| [getWidth()](#getWidth--) | Ottiene la larghezza del frame in unità di 1/4000 dell'area del grafico. |
| [getWidthPixel()](#getWidthPixel--) | Ottiene la larghezza del frame in unità di pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Ottiene la larghezza del frame in unità del rapporto dell'area del grafico. |
| [getX()](#getX--) | Restituisce la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| [getXPixel()](#getXPixel--) | Ottiene la coordinata x dell'angolo superiore sinistro in unità di pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Restituisce la coordinata x dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. |
| [getY()](#getY--) | Ottiene la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| [getYPixel()](#getYPixel--) | Ottiene la coordinata y dell'angolo in alto a sinistra in unità di pixel. |
| [getYRatioToChart()](#getYRatioToChart--) | Restituisce la coordinata y dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indica che il testo è generato automaticamente. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indica se il testo del grafico è ruotato automaticamente. |
| [isAutomaticSize()](#isAutomaticSize--) | Indica se il frame del grafico è dimensionato automaticamente. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [isDeleted()](#isDeleted--) | Indica se questa etichetta dati è eliminata. |
| [isInnerMode()](#isInnerMode--) | Indica se le dimensioni dell'area del grafico includono le tacche e le etichette degli assi. |
| [isNeverOverlap()](#isNeverOverlap--) | Indica se le DataLabels non si sovrappongono mai durante la conversione di un grafico a torta in immagine. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Ottiene se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. |
| [isTextWrapped()](#isTextWrapped--) | Ottiene un valore che indica se il testo è a capo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indica che il testo è generato automaticamente. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indica se il frame del grafico è dimensionato automaticamente. |
| [setBackground(int value)](#setBackground-int-) | Imposta la modalità di visualizzazione dello sfondo. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Imposta la modalità di visualizzazione dello sfondo |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indica se questa etichetta dati è eliminata. |
| [setDirectionType(int value)](#setDirectionType-int-) | Imposta la direzione del testo. |
| [setHeight(int value)](#setHeight-int-) | Imposta l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Imposta l'altezza del frame in unità di pixel. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Imposta l'altezza del frame in unità del rapporto dell'area del grafico. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indica se le dimensioni dell'area del grafico includono le tacche e le etichette degli assi. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Imposta un riferimento al foglio di lavoro. |
| [setNeverOverlap(boolean value)](#setNeverOverlap-boolean-) | Indica se le DataLabels non si sovrappongono mai durante la conversione di un grafico a torta in immagine. |
| [setNumber(int value)](#setNumber-int-) | Imposta il formato numerico incorporato. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Rappresenta la stringa di formato per l'oggetto DataLabels. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | Vero se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle). |
| [setPosition(int value)](#setPosition-int-) | Rappresenta la posizione dell'etichetta dati. |
| [setPositionAuto()](#setPositionAuto--) | Imposta la posizione del frame su automatico |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Rappresenta l'ordine di lettura del testo. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Rappresenta l'angolo di rotazione del testo. |
| [setSeparatorType(int value)](#setSeparatorType-int-) | Imposta il tipo di separatore usato per le etichette dati in un grafico. |
| [setSeparatorValue(String value)](#setSeparatorValue-java.lang.String-) | Imposta il valore del separatore usato per le etichette dati in un grafico. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vero se il frame ha un'ombra. |
| [setShapeType(int value)](#setShapeType-int-) | Imposta il tipo di forma dell'etichetta dati. |
| [setShowBubbleSize(boolean value)](#setShowBubbleSize-boolean-) | Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. |
| [setShowCategoryName(boolean value)](#setShowCategoryName-boolean-) | Rappresenta il comportamento di visualizzazione del nome della categoria dell'etichetta dati di un grafico specificato. Vero per visualizzare il nome della categoria per le etichette dati in un grafico. |
| [setShowCellRange(boolean value)](#setShowCellRange-boolean-) | Indica se mostrare l'intervallo di celle come etichette dati. |
| [setShowLegendKey(boolean value)](#setShowLegendKey-boolean-) | Rappresenta il comportamento di visualizzazione della chiave della legenda dell'etichetta dati di un grafico specificato. |
| [setShowPercentage(boolean value)](#setShowPercentage-boolean-) | Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. |
| [setShowSeriesName(boolean value)](#setShowSeriesName-boolean-) | Indica se il nome della serie viene visualizzato sulle etichette dati in un grafico. |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Rappresenta il comportamento di visualizzazione dei valori dell'etichetta dati di un grafico specificato. |
| [setText(String value)](#setText-java.lang.String-) | Imposta il testo dell'etichetta dati. |
| [setTextDirection(int value)](#setTextDirection-int-) | Rappresenta l'ordine di lettura del testo. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Imposta l'allineamento orizzontale del testo. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Imposta l'allineamento verticale del testo. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Imposta un valore che indica se il testo è a capo. |
| [setWidth(int value)](#setWidth-int-) | Imposta la larghezza del frame in unità di 1/4000 dell'area del grafico. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Imposta la larghezza del frame in unità di Pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Imposta la larghezza del frame in unità di rapporto dell'area del grafico. |
| [setX(int value)](#setX-int-) | Imposta la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| [setXPixel(int value)](#setXPixel-int-) | Imposta la coordinata x dell'angolo in alto a sinistra in unità di Pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Imposta la coordinata x dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. |
| [setY(int value)](#setY-int-) | Imposta la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| [setYPixel(int value)](#setYPixel-int-) | Imposta la coordinata y dell'angolo in alto a sinistra in unità di pixel. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Imposta la coordinata y dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyFont() {#applyFont--}
```
public void applyFont()
```


Applica il carattere delle etichette dati a tutti i nodi figlio.

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | int | L'indice dell'inizio del carattere. |
| length | int | Il numero di caratteri. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
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


Ottiene il [getArea()](../../com.aspose.cells/datalabels\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Ottiene la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartFrame.Area.FillFormat.FillType. Per esempio, se è necessario impostare BackgroundMode su Opaque, è possibile utilizzare il seguente codice: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Questa proprietà sarà rimossa 12 mesi dopo a partire da GENNAIO 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Restituisce la modalità di visualizzazione dello sfondo

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Ottiene il [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Ottiene il grafico a cui appartiene questo oggetto.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


Rappresenta l'altezza della posizione predefinita in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.DefaultHeightRatioToChart, invece. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Rappresenta l'altezza della posizione predefinita in unità della frazione dell'area del grafico.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Rappresenta la larghezza della posizione predefinita in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.DefaultWidthRatioToChart, invece. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Rappresenta la larghezza della posizione predefinita in unità di frazione dell'area del grafico.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Rappresenta x della posizione predefinita in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.DefaultXRatioToChart, invece. DefaultX = (int)(DefaultXRatioToChart \* 4000); Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Rappresenta x della posizione predefinita in unità di frazione dell'area del grafico.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Rappresenta y della posizione predefinita in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.DefaultYRatioToChart, invece. DefaultY = (int)(DefaultYRatioToChart \* 4000); Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Rappresenta y della posizione predefinita in unità della frazione dell'area del grafico.

**Returns:**
double
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Ottiene la direzione del testo.

Vedi [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Ottiene il carattere delle DataLabels;

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Ottiene l'altezza del frame in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.HeightRatioToChart, invece. Height = HeightRatioToChart \* 4000. Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Ottiene l'altezza del frame in unità di pixel.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Ottiene l'altezza del frame in unità del rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è tra 0-1. Come convertire unità di rapporto in pixel? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### getLinkedSource() {#getLinkedSource--}
```
public String getLinkedSource()
```


Ottiene un riferimento al foglio di lavoro.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Ottiene il formato numerico incorporato.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Rappresenta la stringa di formato per l'oggetto DataLabels.

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


Vero se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle).

**Returns:**
boolean
### getPosition() {#getPosition--}
```
public int getPosition()
```


Rappresenta la posizione dell'etichetta dati.

Vedi [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Rappresenta l'ordine di lettura del testo.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Rappresenta l'angolo di rotazione del testo.

**Remarks**


0: Non ruotato.

255: Dall'alto verso il basso.

\-90: Verso il basso.

90: Verso l'alto.


**Returns:**
int
### getSeparatorType() {#getSeparatorType--}
```
public int getSeparatorType()
```


Ottiene il tipo di separatore usato per le etichette dati in un grafico.

Vedi [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Per impostare un separatore personalizzato, impostare la proprietà [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) come [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) e quindi specificare il valore previsto per [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Returns:**
int
### getSeparatorValue() {#getSeparatorValue--}
```
public String getSeparatorValue()
```


Ottiene il valore del separatore usato per le etichette dati in un grafico.

**Returns:**
java.lang.String
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Vero se il frame ha un'ombra.

**Remarks**

Solo per grafici nei file xls.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Ottiene l'oggetto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--).

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getShapeType() {#getShapeType--}
```
public int getShapeType()
```


Ottiene il tipo di forma dell'etichetta dati.

Vedi [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Returns:**
int
### getShowBubbleSize() {#getShowBubbleSize--}
```
public boolean getShowBubbleSize()
```


Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde.

**Returns:**
boolean
### getShowCategoryName() {#getShowCategoryName--}
```
public boolean getShowCategoryName()
```


Rappresenta il comportamento di visualizzazione del nome della categoria dell'etichetta dati di un grafico specificato. True per visualizzare il nome della categoria per le etichette dati su un grafico. False per nasconderlo.

**Returns:**
boolean
### getShowCellRange() {#getShowCellRange--}
```
public boolean getShowCellRange()
```


Indica se mostrare l'intervallo di celle come etichette dati.

**Returns:**
boolean
### getShowLegendKey() {#getShowLegendKey--}
```
public boolean getShowLegendKey()
```


Rappresenta il comportamento di visualizzazione della chiave della legenda dell'etichetta dati di un grafico specificato. True se la chiave della legenda dell'etichetta dati è visibile.

**Returns:**
boolean
### getShowPercentage() {#getShowPercentage--}
```
public boolean getShowPercentage()
```


Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde.

**Returns:**
boolean
### getShowSeriesName() {#getShowSeriesName--}
```
public boolean getShowSeriesName()
```


Indica se il nome della serie viene visualizzato sulle etichette dati di un grafico. True per mostrare il nome della serie. False per nasconderlo.

**Returns:**
boolean
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```


Rappresenta il comportamento di visualizzazione dei valori dell'etichetta dati di un grafico specificato. True visualizza i valori. False li nasconde.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


Ottiene il testo dell'etichetta dati.

**Remarks**

Funziona solo quando si tratta di un'etichetta dati di un punto del grafico.

**Returns:**
java.lang.String
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Rappresenta l'ordine di lettura del testo.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà ChartTextFrame.ReadingOrder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2020. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà ChartFrame.Font. Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


Ottiene l'allineamento orizzontale del testo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Ottiene le opzioni del testo.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


Ottiene l'allineamento verticale del testo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Ottiene la larghezza del frame in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Utilizzare invece la proprietà ChartFrame.WidthRatioToChart. Width = WidthRatioToChart \* 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Ottiene la larghezza del frame in unità di pixel.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Ottiene la larghezza del frame in unità del rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è tra 0 e 1. Come convertire le unità di rapporto in pixel? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Restituisce la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.XRatioToChart, invece. X = XRatioToChart \* 4000. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Ottiene la coordinata x dell'angolo superiore sinistro in unità di pixel.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Restituisce la coordinata x dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è compreso tra 0-1. Come convertire le unità di rapporto in pixel? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Ottiene la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.YRatioToChart, invece. Y = YRatioToChart \* 4000. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Ottiene la coordinata y dell'angolo in alto a sinistra in unità di pixel.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Restituisce la coordinata y dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è compreso tra 0-1. Come convertire le unità di rapporto in pixel? YPixel = YRatioToChart \* Chart.ChartObject.Height;

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoText() {#isAutoText--}
```
public boolean isAutoText()
```


Indica che il testo è generato automaticamente.

**Returns:**
boolean
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Indica se il testo del grafico è ruotato automaticamente.

**Returns:**
boolean
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Indica se il frame del grafico è dimensionato automaticamente.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata.

**Returns:**
boolean
### isDeleted() {#isDeleted--}
```
public boolean isDeleted()
```


Indica se questa etichetta dati è eliminata.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Indica se le dimensioni dell'area del grafico includono i segni di graduazione e le etichette degli assi. False specifica che le dimensioni devono determinare le dimensioni dell'area del grafico, i segni di graduazione e le etichette degli assi.

**Remarks**

Solo per file Xlsx.

**Returns:**
boolean
### isNeverOverlap() {#isNeverOverlap--}
```
public boolean isNeverOverlap()
```


Indica se le etichette dati non si sovrappongono mai durante la conversione di un grafico a torta in immagine. Nota: questa proprietà ha senso solo quando si converte un grafico a torta in immagine.

**Returns:**
boolean
### isResizeShapeToFitText() {#isResizeShapeToFitText--}
```
public boolean isResizeShapeToFitText()
```


Restituisce se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ottiene un valore che indica se il testo è a capo.

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. Il valore predefinito è True.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutoText(boolean value) {#setAutoText-boolean-}
```
public void setAutoText(boolean value)
```


Indica che il testo è generato automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Indica se il frame del grafico è dimensionato automaticamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartFrame.Area.FillFormat.FillType. Per esempio, se è necessario impostare BackgroundMode su Opaque, è possibile utilizzare il seguente codice: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Questa proprietà sarà rimossa 12 mesi dopo a partire da GENNAIO 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Imposta la modalità di visualizzazione dello sfondo

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDeleted(boolean value) {#setDeleted-boolean-}
```
public void setDeleted(boolean value)
```


Indica se questa etichetta dati è eliminata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Imposta la direzione del testo.

Vedi [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Imposta l'altezza del frame in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.HeightRatioToChart, invece. Height = HeightRatioToChart \* 4000. Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Imposta l'altezza del frame in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Imposta l'altezza del frame in unità del rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è tra 0-1. Come convertire unità di rapporto in pixel? HeightPixel = HeightRatioToChart \* Chart.ChartObject.Height;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Indica se le dimensioni dell'area del grafico includono i segni di graduazione e le etichette degli assi. False specifica che le dimensioni devono determinare le dimensioni dell'area del grafico, i segni di graduazione e le etichette degli assi.

**Remarks**

Solo per file Xlsx.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLinkedSource(String value) {#setLinkedSource-java.lang.String-}
```
public void setLinkedSource(String value)
```


Imposta un riferimento al foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNeverOverlap(boolean value) {#setNeverOverlap-boolean-}
```
public void setNeverOverlap(boolean value)
```


Indica se le etichette dati non si sovrappongono mai durante la conversione di un grafico a torta in immagine. Nota: questa proprietà ha senso solo quando si converte un grafico a torta in immagine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Imposta il formato numerico incorporato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Rappresenta la stringa di formato per l'oggetto DataLabels.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


Vero se il formato numerico è collegato alle celle (in modo che il formato numerico cambi nelle etichette quando cambia nelle celle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPosition(int value) {#setPosition-int-}
```
public void setPosition(int value)
```


Rappresenta la posizione dell'etichetta dati.

Vedi [LabelPositionType](../../com.aspose.cells/labelpositiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Imposta la posizione del frame su automatico

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Rappresenta l'ordine di lettura del testo.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setResizeShapeToFitText(boolean value) {#setResizeShapeToFitText-boolean-}
```
public void setResizeShapeToFitText(boolean value)
```


Imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Rappresenta l'angolo di rotazione del testo.

**Remarks**


0: Non ruotato.

255: Dall'alto verso il basso.

\-90: Verso il basso.

90: Verso l'alto.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSeparatorType(int value) {#setSeparatorType-int-}
```
public void setSeparatorType(int value)
```


Imposta il tipo di separatore usato per le etichette dati in un grafico.

Vedi [DataLabelsSeparatorType](../../com.aspose.cells/datalabelsseparatortype).

**Remarks**

Per impostare un separatore personalizzato, impostare la proprietà [getSeparatorType()](../../com.aspose.cells/datalabels\#getSeparatorType--) come [DataLabelsSeparatorType.CUSTOM](../../com.aspose.cells/datalabelsseparatortype\#CUSTOM) e quindi specificare il valore previsto per [getSeparatorValue()](../../com.aspose.cells/datalabels\#getSeparatorValue--).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSeparatorValue(String value) {#setSeparatorValue-java.lang.String-}
```
public void setSeparatorValue(String value)
```


Imposta il valore del separatore usato per le etichette dati in un grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Vero se il frame ha un'ombra.

**Remarks**

Solo per grafici nei file xls.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShapeType(int value) {#setShapeType-int-}
```
public void setShapeType(int value)
```


Imposta il tipo di forma dell'etichetta dati.

Vedi [DataLabelShapeType](../../com.aspose.cells/datalabelshapetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowBubbleSize(boolean value) {#setShowBubbleSize-boolean-}
```
public void setShowBubbleSize(boolean value)
```


Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowCategoryName(boolean value) {#setShowCategoryName-boolean-}
```
public void setShowCategoryName(boolean value)
```


Rappresenta il comportamento di visualizzazione del nome della categoria dell'etichetta dati di un grafico specificato. True per visualizzare il nome della categoria per le etichette dati su un grafico. False per nasconderlo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowCellRange(boolean value) {#setShowCellRange-boolean-}
```
public void setShowCellRange(boolean value)
```


Indica se mostrare l'intervallo di celle come etichette dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowLegendKey(boolean value) {#setShowLegendKey-boolean-}
```
public void setShowLegendKey(boolean value)
```


Rappresenta il comportamento di visualizzazione della chiave della legenda dell'etichetta dati di un grafico specificato. True se la chiave della legenda dell'etichetta dati è visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowPercentage(boolean value) {#setShowPercentage-boolean-}
```
public void setShowPercentage(boolean value)
```


Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowSeriesName(boolean value) {#setShowSeriesName-boolean-}
```
public void setShowSeriesName(boolean value)
```


Indica se il nome della serie viene visualizzato sulle etichette dati di un grafico. True per mostrare il nome della serie. False per nasconderlo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```


Rappresenta il comportamento di visualizzazione dei valori dell'etichetta dati di un grafico specificato. True visualizza i valori. False li nasconde.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Imposta il testo dell'etichetta dati.

**Remarks**

Funziona solo quando si tratta di un'etichetta dati di un punto del grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Rappresenta l'ordine di lettura del testo.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà ChartTextFrame.ReadingOrder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2020. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Imposta l'allineamento orizzontale del testo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Imposta l'allineamento verticale del testo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Imposta un valore che indica se il testo è a capo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Imposta la larghezza del frame in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Utilizzare invece la proprietà ChartFrame.WidthRatioToChart. Width = WidthRatioToChart \* 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Imposta la larghezza del frame in unità di Pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Imposta la larghezza del frame in unità di rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è tra 0 e 1. Come convertire le unità di rapporto in pixel? WidthPixel = WidthRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Imposta la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.XRatioToChart, invece. X = XRatioToChart \* 4000. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Imposta la coordinata x dell'angolo in alto a sinistra in unità di Pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Imposta la coordinata x dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è compreso tra 0-1. Come convertire le unità di rapporto in pixel? XPixel = XRatioToChart \* Chart.ChartObject.Width;

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Imposta la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.YRatioToChart, invece. Y = YRatioToChart \* 4000. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Imposta la coordinata y dell'angolo in alto a sinistra in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Imposta la coordinata y dell'angolo in alto a sinistra in unità di rapporto dell'area del grafico.

**Remarks**

Questo è un valore frazionario, il suo intervallo valido è compreso tra 0-1. Come convertire le unità di rapporto in pixel? YPixel = YRatioToChart \* Chart.ChartObject.Height;

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

