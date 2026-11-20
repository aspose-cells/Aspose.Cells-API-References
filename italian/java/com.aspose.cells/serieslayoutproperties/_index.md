---
title: "SeriesLayoutProperties"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le proprietà del layout della serie."
type: docs
url: /it/java/com.aspose.cells/serieslayoutproperties/
---

**Inheritance:**
java.lang.Object
```
public class SeriesLayoutProperties
```

Rappresenta le proprietà del layout della serie.

**Remarks**

Applicabile solo a grafici BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall e Histogram.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SeriesLayoutProperties()](#SeriesLayoutProperties--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMapChartProjectionType()](#getMapChartProjectionType--) | Ottiene il tipo di proiezione della mappa. |
| [getMapChartRegionType()](#getMapChartRegionType--) | Ottiene il tipo di regione della mappa. |
| [getMapLabelLayout()](#getMapLabelLayout--) | Ottiene il layout delle etichette della mappa. |
| [getQuartileCalculation()](#getQuartileCalculation--) | Rappresenta le proprietà statistiche per la serie. |
| [getShowConnectorLines()](#getShowConnectorLines--) | Indica se le linee di collegamento sono visualizzate tra i punti dati. |
| [getShowInnerPoints()](#getShowInnerPoints--) | Indica se mostrare i punti dati non anomali. |
| [getShowMeanLine()](#getShowMeanLine--) | Indica se mostrare la linea che collega tutti i punti medio. |
| [getShowMeanMarker()](#getShowMeanMarker--) | Indica se i marcatori che indicano la media sono mostrati. |
| [getShowOutlierPoints()](#getShowOutlierPoints--) | Indica se i punti dati anomali sono mostrati. |
| [getSubtotals()](#getSubtotals--) | Rappresenta l'indice di un punto dati subtotale. |
| [hashCode()](#hashCode--) |  |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--) | Indica se l'intervallo è chiuso sul lato sinistro. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIntervalLeftClosed(boolean value)](#setIntervalLeftClosed-boolean-) | Indica se l'intervallo è chiuso sul lato sinistro. |
| [setMapChartProjectionType(int value)](#setMapChartProjectionType-int-) | Imposta il tipo di proiezione della mappa. |
| [setMapChartRegionType(int value)](#setMapChartRegionType-int-) | Imposta il tipo di regione della mappa. |
| [setMapLabelLayout(int value)](#setMapLabelLayout-int-) | Imposta il layout delle etichette della mappa. |
| [setQuartileCalculation(int value)](#setQuartileCalculation-int-) | Rappresenta le proprietà statistiche per la serie. |
| [setShowConnectorLines(boolean value)](#setShowConnectorLines-boolean-) | Indica se le linee di collegamento sono visualizzate tra i punti dati. |
| [setShowInnerPoints(boolean value)](#setShowInnerPoints-boolean-) | Indica se mostrare i punti dati non anomali. |
| [setShowMeanLine(boolean value)](#setShowMeanLine-boolean-) | Indica se mostrare la linea che collega tutti i punti medio. |
| [setShowMeanMarker(boolean value)](#setShowMeanMarker-boolean-) | Indica se i marcatori che indicano la media sono mostrati. |
| [setShowOutlierPoints(boolean value)](#setShowOutlierPoints-boolean-) | Indica se i punti dati anomali sono mostrati. |
| [setSubtotals(int[] value)](#setSubtotals-int---) | Rappresenta l'indice di un punto dati subtotale. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SeriesLayoutProperties() {#SeriesLayoutProperties--}
```
public SeriesLayoutProperties()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getMapChartProjectionType() {#getMapChartProjectionType--}
```
public int getMapChartProjectionType()
```


Ottiene il tipo di proiezione della mappa.

Vedi [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Solo per grafico mappa.

**Returns:**
int
### getMapChartRegionType() {#getMapChartRegionType--}
```
public int getMapChartRegionType()
```


Ottiene il tipo di regione della mappa.

Vedi [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Solo per grafico mappa.

**Returns:**
int
### getMapLabelLayout() {#getMapLabelLayout--}
```
public int getMapLabelLayout()
```


Ottiene il layout delle etichette della mappa.

Vedi [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Returns:**
int
### getQuartileCalculation() {#getQuartileCalculation--}
```
public int getQuartileCalculation()
```


Rappresenta le proprietà statistiche per la serie.

Vedi [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Applicabile solo al grafico BoxWhisker.

**Returns:**
int
### getShowConnectorLines() {#getShowConnectorLines--}
```
public boolean getShowConnectorLines()
```


Indica se le linee di collegamento sono visualizzate tra i punti dati.

**Remarks**

Solo per grafico Waterfall.

**Returns:**
boolean
### getShowInnerPoints() {#getShowInnerPoints--}
```
public boolean getShowInnerPoints()
```


Indica se mostrare i punti dati non anomali.

**Returns:**
boolean
### getShowMeanLine() {#getShowMeanLine--}
```
public boolean getShowMeanLine()
```


Indica se mostrare la linea che collega tutti i punti medio.

**Remarks**

Funziona solo per grafico BoxWhisker.

**Returns:**
boolean
### getShowMeanMarker() {#getShowMeanMarker--}
```
public boolean getShowMeanMarker()
```


Indica se i marcatori che indicano la media sono mostrati.

**Returns:**
boolean
### getShowOutlierPoints() {#getShowOutlierPoints--}
```
public boolean getShowOutlierPoints()
```


Indica se i punti dati anomali sono mostrati.

**Returns:**
boolean
### getSubtotals() {#getSubtotals--}
```
public int[] getSubtotals()
```


Rappresenta l'indice di un punto dati subtotale.

**Returns:**
int[]
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isIntervalLeftClosed() {#isIntervalLeftClosed--}
```
public boolean isIntervalLeftClosed()
```


Indica se l'intervallo è chiuso sul lato sinistro.

**Remarks**

Solo per grafico ParetoLine.

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




### setIntervalLeftClosed(boolean value) {#setIntervalLeftClosed-boolean-}
```
public void setIntervalLeftClosed(boolean value)
```


Indica se l'intervallo è chiuso sul lato sinistro.

**Remarks**

Solo per grafico ParetoLine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setMapChartProjectionType(int value) {#setMapChartProjectionType-int-}
```
public void setMapChartProjectionType(int value)
```


Imposta il tipo di proiezione della mappa.

Vedi [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Solo per grafico mappa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMapChartRegionType(int value) {#setMapChartRegionType-int-}
```
public void setMapChartRegionType(int value)
```


Imposta il tipo di regione della mappa.

Vedi [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Solo per grafico mappa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setMapLabelLayout(int value) {#setMapLabelLayout-int-}
```
public void setMapLabelLayout(int value)
```


Imposta il layout delle etichette della mappa.

Vedi [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setQuartileCalculation(int value) {#setQuartileCalculation-int-}
```
public void setQuartileCalculation(int value)
```


Rappresenta le proprietà statistiche per la serie.

Vedi [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Applicabile solo al grafico BoxWhisker.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShowConnectorLines(boolean value) {#setShowConnectorLines-boolean-}
```
public void setShowConnectorLines(boolean value)
```


Indica se le linee di collegamento sono visualizzate tra i punti dati.

**Remarks**

Solo per grafico Waterfall.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowInnerPoints(boolean value) {#setShowInnerPoints-boolean-}
```
public void setShowInnerPoints(boolean value)
```


Indica se mostrare i punti dati non anomali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowMeanLine(boolean value) {#setShowMeanLine-boolean-}
```
public void setShowMeanLine(boolean value)
```


Indica se mostrare la linea che collega tutti i punti medio.

**Remarks**

Funziona solo per grafico BoxWhisker.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowMeanMarker(boolean value) {#setShowMeanMarker-boolean-}
```
public void setShowMeanMarker(boolean value)
```


Indica se i marcatori che indicano la media sono mostrati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setShowOutlierPoints(boolean value) {#setShowOutlierPoints-boolean-}
```
public void setShowOutlierPoints(boolean value)
```


Indica se i punti dati anomali sono mostrati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSubtotals(int[] value) {#setSubtotals-int---}
```
public void setSubtotals(int[] value)
```


Rappresenta l'indice di un punto dati subtotale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int[] |  |

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

