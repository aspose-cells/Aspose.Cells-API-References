---
title: "Walls"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta le pareti di un grafico 3-D."
type: docs
url: /it/java/com.aspose.cells/walls/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Area](../../com.aspose.cells/area), [com.aspose.cells.Floor](../../com.aspose.cells/floor)
```
public class Walls extends Floor
```

Incapsula l'oggetto che rappresenta le pareti di un grafico 3-D.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackgroundColor()](#getBackgroundColor--) | Ottiene il [Color](../../com.aspose.cells/color) di sfondo dell'[Area](../../com.aspose.cells/area). |
| [getBorder()](#getBorder--) | Ottiene il bordo [Line](../../com.aspose.cells/line). |
| [getCenterX()](#getCenterX--) | Restituisce la coordinata x dell'angolo sinistro‑inferiore del centro del Muro in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate(). |
| [getCenterXPx()](#getCenterXPx--) | Restituisce la coordinata x dell'angolo inferiore‑sinistro del centro del Muro in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [getCenterY()](#getCenterY--) | Restituisce la coordinata y dell'angolo sinistro‑inferiore del centro del Muro in unità di 1/4000 dell'altezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [getCenterYPx()](#getCenterYPx--) | Restituisce la coordinata y dell'angolo sinistro‑inferiore del centro del Muro in unità di pixel dopo le chiamate al metodo Chart.Calculate(). |
| [getClass()](#getClass--) |  |
| [getCubePointCount()](#getCubePointCount--) | Restituisce il numero di punti del cubo dopo le chiamate al metodo Chart.Calculate(). |
| [getCubePointXPx(int index)](#getCubePointXPx-int-) | Restituisce la coordinata x del punto apice del cubo dei muri dopo la chiamata al metodo Chart.Calculate(). |
| [getCubePointYPx(int index)](#getCubePointYPx-int-) | Restituisce la coordinata y del punto apice del cubo dei muri dopo le chiamate al metodo Chart.Calculate(). |
| [getDepth()](#getDepth--) | Restituisce la profondità da davanti a dietro in unità di 1/4000 della larghezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [getDepthPx()](#getDepthPx--) | Restituisce la profondità da davanti a dietro in unità di pixel dopo le chiamate al metodo Chart.Calculate(). |
| [getFillFormat()](#getFillFormat--) | Rappresenta un oggetto [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) che contiene le proprietà di formattazione di riempimento per il grafico o la forma specificati. |
| [getForegroundColor()](#getForegroundColor--) | Ottiene il [Color](../../com.aspose.cells/color) in primo piano. |
| [getFormatting()](#getFormatting--) | Rappresenta la formattazione dell'area. |
| [getHeight()](#getHeight--) | Restituisce l'altezza dall'alto verso il basso in unità di 1/4000 dell'altezza del grafico dopo le chiamate al metodo Chart.Calculate(). |
| [getHeightPx()](#getHeightPx--) | Restituisce l'altezza dall'alto verso il basso in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [getInvertIfNegative()](#getInvertIfNegative--) | Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati. |
| [getTransparency()](#getTransparency--) | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
| [getWidth()](#getWidth--) | Restituisce la larghezza da sinistra a destra in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate(). |
| [getWidthPx()](#getWidthPx--) | Restituisce la larghezza da sinistra a destra in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Imposta il [Color](../../com.aspose.cells/color) di sfondo dell'[Area](../../com.aspose.cells/area). |
| [setBorder(Line value)](#setBorder-com.aspose.cells.Line-) | Imposta il bordo [Line](../../com.aspose.cells/line). |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Imposta il [Color](../../com.aspose.cells/color) in primo piano. |
| [setFormatting(int value)](#setFormatting-int-) | Rappresenta la formattazione dell'area. |
| [setInvertIfNegative(boolean value)](#setInvertIfNegative-boolean-) | Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati. |
| [setTransparency(double value)](#setTransparency-double-) | Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente). |
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
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Ottiene il [Color](../../com.aspose.cells/color) di sfondo dell'[Area](../../com.aspose.cells/area).

**Returns:**
[Color](../../com.aspose.cells/color)
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Ottiene il bordo [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getCenterX() {#getCenterX--}
```
public int getCenterX()
```


Restituisce la coordinata x dell'angolo sinistro‑inferiore del centro del Muro in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate().

**Returns:**
int
### getCenterXPx() {#getCenterXPx--}
```
public int getCenterXPx()
```


Restituisce la coordinata x dell'angolo inferiore‑sinistro del centro del Muro in unità di pixel dopo la chiamata al metodo Chart.Calculate().

**Returns:**
int
### getCenterY() {#getCenterY--}
```
public int getCenterY()
```


Restituisce la coordinata y dell'angolo sinistro‑inferiore del centro del Muro in unità di 1/4000 dell'altezza del grafico dopo la chiamata al metodo Chart.Calculate().

**Returns:**
int
### getCenterYPx() {#getCenterYPx--}
```
public int getCenterYPx()
```


Restituisce la coordinata y dell'angolo sinistro‑inferiore del centro del Muro in unità di pixel dopo le chiamate al metodo Chart.Calculate().

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCubePointCount() {#getCubePointCount--}
```
public int getCubePointCount()
```


Restituisce il numero di punti del cubo dopo le chiamate al metodo Chart.Calculate().

**Returns:**
int
### getCubePointXPx(int index) {#getCubePointXPx-int-}
```
public float getCubePointXPx(int index)
```


Restituisce la coordinata x del punto apice del cubo dei muri dopo la chiamata al metodo Chart.Calculate(). Il numero di punti apice del cubo dei muri è otto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
float
### getCubePointYPx(int index) {#getCubePointYPx-int-}
```
public float getCubePointYPx(int index)
```


Restituisce la coordinata y del punto apice del cubo dei muri dopo le chiamate al metodo Chart.Calculate(). Il numero di punti apice del cubo dei muri è otto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
float
### getDepth() {#getDepth--}
```
public int getDepth()
```


Restituisce la profondità da davanti a dietro in unità di 1/4000 della larghezza del grafico dopo la chiamata al metodo Chart.Calculate().

**Returns:**
int
### getDepthPx() {#getDepthPx--}
```
public int getDepthPx()
```


Restituisce la profondità da davanti a dietro in unità di pixel dopo le chiamate al metodo Chart.Calculate().

**Returns:**
int
### getFillFormat() {#getFillFormat--}
```
public FillFormat getFillFormat()
```


Rappresenta un oggetto [getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) che contiene le proprietà di formattazione di riempimento per il grafico o la forma specificati.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Ottiene il [Color](../../com.aspose.cells/color) in primo piano.

**Returns:**
[Color](../../com.aspose.cells/color)
### getFormatting() {#getFormatting--}
```
public int getFormatting()
```


Rappresenta la formattazione dell'area.

Vedi [FormattingType](../../com.aspose.cells/formattingtype).

**Returns:**
int
### getHeight() {#getHeight--}
```
public int getHeight()
```


Restituisce l'altezza dall'alto verso il basso in unità di 1/4000 dell'altezza del grafico dopo le chiamate al metodo Chart.Calculate().

**Returns:**
int
### getHeightPx() {#getHeightPx--}
```
public int getHeightPx()
```


Restituisce l'altezza dall'alto verso il basso in unità di pixel dopo la chiamata al metodo Chart.Calculate().

**Returns:**
int
### getInvertIfNegative() {#getInvertIfNegative--}
```
public boolean getInvertIfNegative()
```


Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(-100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
         chart.getNSeries().add("A1:A3", true);
         boolean isNegative = chart.getNSeries().get(0).getArea().getInvertIfNegative();
         chart.getNSeries().get(0).getArea().setInvertIfNegative(true);
         //Setting the foreground color of the 1st NSeries area
         chart.getNSeries().get(0).getArea().setForegroundColor(Color.getRed());
         //Setting the background color of the 1st NSeries area.
         //The displayed area color of second chart point will be the background color.
         chart.getNSeries().get(0).getArea().setBackgroundColor(Color.getYellow());
         //Saving the Excel file
         workbook.save("book1.xls");
```

**Returns:**
boolean
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

**Returns:**
double
### getWidth() {#getWidth--}
```
public int getWidth()
```


Restituisce la larghezza da sinistra a destra in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate().

**Returns:**
int
### getWidthPx() {#getWidthPx--}
```
public int getWidthPx()
```


Restituisce la larghezza da sinistra a destra in unità di pixel dopo la chiamata al metodo Chart.Calculate().

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Imposta il [Color](../../com.aspose.cells/color) di sfondo dell'[Area](../../com.aspose.cells/area).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBorder(Line value) {#setBorder-com.aspose.cells.Line-}
```
public void setBorder(Line value)
```


Imposta il bordo [Line](../../com.aspose.cells/line).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Line](../../com.aspose.cells/line) |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Imposta il [Color](../../com.aspose.cells/color) in primo piano.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setFormatting(int value) {#setFormatting-int-}
```
public void setFormatting(int value)
```


Rappresenta la formattazione dell'area.

Vedi [FormattingType](../../com.aspose.cells/formattingtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setInvertIfNegative(boolean value) {#setInvertIfNegative-boolean-}
```
public void setInvertIfNegative(boolean value)
```


Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

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

