---
title: "ChartFrame"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta l'oggetto frame in un grafico."
type: docs
url: /it/java/com.aspose.cells/chartframe/
---

**Inheritance:**
java.lang.Object
```
public class ChartFrame
```

Incapsula l'oggetto che rappresenta l'oggetto frame in un grafico.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Ottiene il [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [getBackground()](#getBackground--) | Ottiene la modalità di visualizzazione dello sfondo. |
| [getBackgroundMode()](#getBackgroundMode--) | Ottiene la modalità di visualizzazione dello sfondo. |
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
| [getFont()](#getFont--) | Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato. |
| [getHeight()](#getHeight--) | Ottiene l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| [getHeightPixel()](#getHeightPixel--) | Ottiene l'altezza del frame in unità di pixel. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Ottiene l'altezza del frame in unità del rapporto dell'area del grafico. |
| [getShadow()](#getShadow--) | Vero se il frame ha un'ombra. |
| [getShapeProperties()](#getShapeProperties--) | Ottiene l'oggetto [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getTextFont()](#getTextFont--) | Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato. |
| [getTextOptions()](#getTextOptions--) | Ottiene le opzioni del testo. |
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
| [isAutomaticSize()](#isAutomaticSize--) | Indica se il frame del grafico è dimensionato automaticamente. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata. |
| [isInnerMode()](#isInnerMode--) | Indica se le dimensioni dell'area del grafico includono le tacche e le etichette degli assi. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True se il testo nell'oggetto cambia la dimensione del carattere quando la dimensione dell'oggetto cambia. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indica se il frame del grafico è dimensionato automaticamente. |
| [setBackground(int value)](#setBackground-int-) | Imposta la modalità di visualizzazione dello sfondo. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Imposta la modalità di visualizzazione dello sfondo. |
| [setHeight(int value)](#setHeight-int-) | Imposta l'altezza del frame in unità di 1/4000 dell'area del grafico. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Imposta l'altezza del frame in unità di pixel. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Imposta l'altezza del frame in unità del rapporto dell'area del grafico. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indica se le dimensioni dell'area del grafico includono le tacche e le etichette degli assi. |
| [setPositionAuto()](#setPositionAuto--) | Imposta la posizione del frame su automatico |
| [setShadow(boolean value)](#setShadow-boolean-) | Vero se il frame ha un'ombra. |
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
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Ottiene un oggetto [getFont()](../../com.aspose.cells/chartframe\#getFont--) del ChartFrame specificato.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà ChartFrame.Font. Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2012. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Ottiene le opzioni del testo.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
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
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Indica se le dimensioni dell'area del grafico includono i segni di graduazione e le etichette degli assi. False specifica che le dimensioni devono determinare le dimensioni dell'area del grafico, i segni di graduazione e le etichette degli assi.

**Remarks**

Solo per file Xlsx.

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

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Imposta la posizione del frame su automatico

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

