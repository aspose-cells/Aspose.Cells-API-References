---
title: "Title"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta il titolo del grafico o dell'asse."
type: docs
url: /it/java/com.aspose.cells/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe), [com.aspose.cells.ChartTextFrame](../../com.aspose.cells/charttextframe)
```
public class Title extends ChartTextFrame
```

Incapsula l'oggetto che rappresenta il titolo del grafico o dell'asse.

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
 
         	int chartIndex = sheet.getCharts().add(ChartType.COLUMN, 9, 9, 21, 15);
         	Chart chart = sheet.getCharts().get(chartIndex);
 
         //Setting the title of a chart
         chart.getTitle().setText("Title");
         //Setting the font color of the chart title to blue
         chart.getTitle().getFont().setColor(Color.getBlue());
         //Setting the title of category axis of the chart
         chart.getCategoryAxis().getTitle().setText("Category");
         //Setting the title of value axis of the chart
         chart.getValueAxis().getTitle().setText("Value");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [characters()](#characters--) | Ottiene la formattazione del testo ricco di questo Title. |
| [characters(int startIndex, int length)](#characters-int-int-) | Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Ottiene il [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [getBackground()](#getBackground--) | Ottiene la modalità di visualizzazione dello sfondo. |
| [getBackgroundMode()](#getBackgroundMode--) | Ottiene la modalità di visualizzazione dello sfondo. |
| [getBorder()](#getBorder--) | Ottiene il [Line](../../com.aspose.cells/line). |
| [getCharacters()](#getCharacters--) | Ottiene la formattazione del testo ricco di questo Title. |
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
| [getFont()](#getFont--) | Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato. |
| [getHeight()](#getHeight--) | Ottiene l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| [getHeightPixel()](#getHeightPixel--) | Ottiene l'altezza del frame in unità di pixel. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Ottiene l'altezza del frame in unità del rapporto dell'area del grafico. |
| [getLinkedSource()](#getLinkedSource--) | Ottiene un riferimento al foglio di lavoro. |
| [getOverLay()](#getOverLay--) | Rappresenta un titolo sovrapposto centrato su un grafico senza ridimensionare il grafico. |
| [getReadingOrder()](#getReadingOrder--) | Rappresenta l'ordine di lettura del testo. |
| [getRotationAngle()](#getRotationAngle--) | Rappresenta l'angolo di rotazione del testo. |
| [getShadow()](#getShadow--) | Vero se il frame ha un'ombra. |
| [getShapeProperties()](#getShapeProperties--) | Ottiene l'oggetto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getText()](#getText--) | Ottiene il testo dell'etichetta dell'unità di visualizzazione. |
| [getTextDirection()](#getTextDirection--) | Rappresenta l'ordine di lettura del testo. |
| [getTextFont()](#getTextFont--) | Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Ottiene l'allineamento orizzontale del testo. |
| [getTextOptions()](#getTextOptions--) | Ottiene le opzioni del testo. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Ottiene l'allineamento verticale del testo. |
| [getWidth()](#getWidth--) | Ottiene la larghezza del frame in unità di 1/4000 dell'area del grafico. |
| [getWidthPixel()](#getWidthPixel--) | Ottiene la larghezza del frame in unità di pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Ottiene la larghezza del frame in unità del rapporto dell'area del grafico. |
| [getX()](#getX--) | Ottiene la coordinata X dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico. |
| [getXPixel()](#getXPixel--) | Ottiene la coordinata x dell'angolo superiore sinistro in unità di pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Ottiene la coordinata x dell'angolo in alto a sinistra in unità di Frazione dell'area del grafico. |
| [getY()](#getY--) | Ottiene la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| [getYPixel()](#getYPixel--) | Ottiene la coordinata y dell'angolo in alto a sinistra in unità di pixel. |
| [getYRatioToChart()](#getYRatioToChart--) | Ottiene la coordinata y dell'angolo in alto a sinistra in unità di Frazione dell'area del grafico. |
| [hashCode()](#hashCode--) |  |
| [isAutoText()](#isAutoText--) | Indica che il testo è generato automaticamente. |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indica se il testo del grafico è ruotato automaticamente. |
| [isAutomaticSize()](#isAutomaticSize--) | Indica se il frame del grafico è dimensionato automaticamente. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [isDeleted()](#isDeleted--) | Indica se questa etichetta dati è eliminata. |
| [isInnerMode()](#isInnerMode--) | Indica se le dimensioni dell'area del grafico includono le tacche e le etichette degli assi. |
| [isResizeShapeToFitText()](#isResizeShapeToFitText--) | Ottiene se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. |
| [isTextWrapped()](#isTextWrapped--) | Ottiene un valore che indica se il testo è a capo. |
| [isVisible()](#isVisible--) | Rappresenta se il titolo è visibile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [setAutoText(boolean value)](#setAutoText-boolean-) | Indica che il testo è generato automaticamente. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indica se il frame del grafico è dimensionato automaticamente. |
| [setBackground(int value)](#setBackground-int-) | Imposta la modalità di visualizzazione dello sfondo. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Imposta la modalità di visualizzazione dello sfondo. |
| [setDeleted(boolean value)](#setDeleted-boolean-) | Indica se questa etichetta dati è eliminata. |
| [setDirectionType(int value)](#setDirectionType-int-) | Imposta la direzione del testo. |
| [setHeight(int value)](#setHeight-int-) | Imposta l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Imposta l'altezza del frame in unità di pixel. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Imposta l'altezza del frame in unità del rapporto dell'area del grafico. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indica se le dimensioni dell'area del grafico includono le tacche e le etichette degli assi. |
| [setLinkedSource(String value)](#setLinkedSource-java.lang.String-) | Imposta un riferimento al foglio di lavoro. |
| [setOverLay(boolean value)](#setOverLay-boolean-) | Rappresenta un titolo sovrapposto centrato su un grafico senza ridimensionare il grafico. |
| [setPositionAuto()](#setPositionAuto--) | Imposta la posizione del frame su automatico |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Rappresenta l'ordine di lettura del testo. |
| [setResizeShapeToFitText(boolean value)](#setResizeShapeToFitText-boolean-) | Imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Rappresenta l'angolo di rotazione del testo. |
| [setShadow(boolean value)](#setShadow-boolean-) | Vero se il frame ha un'ombra. |
| [setText(String value)](#setText-java.lang.String-) | Imposta il testo dell'etichetta dell'unità di visualizzazione. |
| [setTextDirection(int value)](#setTextDirection-int-) | Rappresenta l'ordine di lettura del testo. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Imposta l'allineamento orizzontale del testo. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Imposta l'allineamento verticale del testo. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Imposta un valore che indica se il testo è a capo. |
| [setVisible(boolean value)](#setVisible-boolean-) | Rappresenta se il titolo è visibile. |
| [setWidth(int value)](#setWidth-int-) | Imposta la larghezza del frame in unità di 1/4000 dell'area del grafico. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Imposta la larghezza del frame in unità di Pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Imposta la larghezza del frame in unità di rapporto dell'area del grafico. |
| [setX(int value)](#setX-int-) | Imposta la coordinata X dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| [setXPixel(int value)](#setXPixel-int-) | Imposta la coordinata x dell'angolo in alto a sinistra in unità di Pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Imposta la coordinata x dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. |
| [setY(int value)](#setY-int-) | Imposta la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico. |
| [setYPixel(int value)](#setYPixel-int-) | Imposta la coordinata y dell'angolo in alto a sinistra in unità di pixel. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Imposta la coordinata y dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### characters() {#characters--}
```
public FontSetting[] characters()
```


Ottiene la formattazione del testo ricco di questo Title.

**Returns:**
com.aspose.cells.FontSetting[] - restituisce un array di FontSetting
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


Ottiene il [getArea()](../../com.aspose.cells/chartframe\#getArea--).

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


Ottiene la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartFrame.Area.FillFormat.FillType. Per esempio, se è necessario impostare BackgroundMode su Opaque, è possibile utilizzare il seguente codice: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Ottiene il [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Ottiene la formattazione del testo ricco di questo Title.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Title.Characters(). Questa proprietà sarà rimossa 12 mesi dopo a partire da novembre 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
com.aspose.cells.FontSetting[] - restituisce un array di FontSetting
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


Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato.

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
### getOverLay() {#getOverLay--}
```
public boolean getOverLay()
```


Rappresenta un titolo sovrapposto centrato su un grafico senza ridimensionare il grafico.

**Returns:**
boolean
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
### getText() {#getText--}
```
public String getText()
```


Ottiene il testo dell'etichetta dell'unità di visualizzazione.

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


Ottiene la coordinata X dell'angolo superiore sinistro in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Utilizzare invece la proprietà Title.XRatioToChart. X = XRatioToChart \* 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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


Restituisce la coordinata x dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. X in pixel = XRatioToChart \* Chart.ChartObject.Width;

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Ottiene la coordinata y dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Utilizzare invece la proprietà Title.YRatioToChart. Y = YRatioToChart \* 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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


Restituisce la coordinata y dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. Y in pixel = YRatioToChart \* Chart.ChartObject.Width;

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
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Rappresenta se il titolo è visibile.

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


Imposta la modalità di visualizzazione dello sfondo. Questa proprietà è valida solo in Excel 2003 o versioni precedenti.

Vedi [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ChartFrame.Area.FillFormat.FillType. Per esempio, se è necessario impostare BackgroundMode su Opaque, è possibile utilizzare il seguente codice: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Questa proprietà sarà rimossa 12 mesi dopo a partire da febbraio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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

### setOverLay(boolean value) {#setOverLay-boolean-}
```
public void setOverLay(boolean value)
```


Rappresenta un titolo sovrapposto centrato su un grafico senza ridimensionare il grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Imposta il testo dell'etichetta dell'unità di visualizzazione.

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

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Rappresenta se il titolo è visibile.

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


Imposta la coordinata X dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

**Remarks**

NOTA: Questo membro è ora obsoleto. Utilizzare invece la proprietà Title.XRatioToChart. X = XRatioToChart \* 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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


Imposta la coordinata x dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. X in pixel = XRatioToChart \* Chart.ChartObject.Width;

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

NOTA: Questo membro è ora obsoleto. Utilizzare invece la proprietà Title.YRatioToChart. Y = YRatioToChart \* 4000; Questa proprietà sarà rimossa 12 mesi dopo, a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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


Imposta la coordinata y dell'angolo in alto a sinistra in unità di frazione dell'area del grafico. Y in pixel = YRatioToChart \* Chart.ChartObject.Width;

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

