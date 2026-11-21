---
title: "SeriesLayoutProperties"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa las propiedades del diseño de series."
type: docs
url: /es/java/com.aspose.cells/serieslayoutproperties/
---

**Inheritance:**
java.lang.Object
```
public class SeriesLayoutProperties
```

Representa las propiedades del diseño de series.

**Remarks**

Solo aplicable a los gráficos BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall y Histogram.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SeriesLayoutProperties()](#SeriesLayoutProperties--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMapChartProjectionType()](#getMapChartProjectionType--) | Obtiene el tipo de proyección del mapa. |
| [getMapChartRegionType()](#getMapChartRegionType--) | Obtiene el tipo de región del mapa. |
| [getMapLabelLayout()](#getMapLabelLayout--) | Obtiene el diseño de las etiquetas del mapa. |
| [getQuartileCalculation()](#getQuartileCalculation--) | Representa las propiedades estadísticas de la serie. |
| [getShowConnectorLines()](#getShowConnectorLines--) | Indica si se muestran líneas de conexión entre los puntos de datos. |
| [getShowInnerPoints()](#getShowInnerPoints--) | Indica si se muestran los puntos de datos que no son valores atípicos. |
| [getShowMeanLine()](#getShowMeanLine--) | Indica si se muestra la línea que conecta todos los puntos de media. |
| [getShowMeanMarker()](#getShowMeanMarker--) | Indica si se muestran los marcadores que denotan la media. |
| [getShowOutlierPoints()](#getShowOutlierPoints--) | Indica si se muestran los puntos de datos atípicos. |
| [getSubtotals()](#getSubtotals--) | Representa el índice de un punto de datos subtotal. |
| [hashCode()](#hashCode--) |  |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--) | Indica si el intervalo está cerrado en el lado izquierdo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIntervalLeftClosed(boolean value)](#setIntervalLeftClosed-boolean-) | Indica si el intervalo está cerrado en el lado izquierdo. |
| [setMapChartProjectionType(int value)](#setMapChartProjectionType-int-) | Establece el tipo de proyección del mapa. |
| [setMapChartRegionType(int value)](#setMapChartRegionType-int-) | Establece el tipo de región del mapa. |
| [setMapLabelLayout(int value)](#setMapLabelLayout-int-) | Establece el diseño de las etiquetas del mapa. |
| [setQuartileCalculation(int value)](#setQuartileCalculation-int-) | Representa las propiedades estadísticas de la serie. |
| [setShowConnectorLines(boolean value)](#setShowConnectorLines-boolean-) | Indica si se muestran líneas de conexión entre los puntos de datos. |
| [setShowInnerPoints(boolean value)](#setShowInnerPoints-boolean-) | Indica si se muestran los puntos de datos que no son valores atípicos. |
| [setShowMeanLine(boolean value)](#setShowMeanLine-boolean-) | Indica si se muestra la línea que conecta todos los puntos de media. |
| [setShowMeanMarker(boolean value)](#setShowMeanMarker-boolean-) | Indica si se muestran los marcadores que denotan la media. |
| [setShowOutlierPoints(boolean value)](#setShowOutlierPoints-boolean-) | Indica si se muestran los puntos de datos atípicos. |
| [setSubtotals(int[] value)](#setSubtotals-int---) | Representa el índice de un punto de datos subtotal. |
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
| Parámetro | Tipo | Descripción |
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


Obtiene el tipo de proyección del mapa.

Ver [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Solo para gráfico de mapa.

**Returns:**
int
### getMapChartRegionType() {#getMapChartRegionType--}
```
public int getMapChartRegionType()
```


Obtiene el tipo de región del mapa.

Ver [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Solo para gráfico de mapa.

**Returns:**
int
### getMapLabelLayout() {#getMapLabelLayout--}
```
public int getMapLabelLayout()
```


Obtiene el diseño de las etiquetas del mapa.

Ver [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Returns:**
int
### getQuartileCalculation() {#getQuartileCalculation--}
```
public int getQuartileCalculation()
```


Representa las propiedades estadísticas de la serie.

Ver [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Solo aplicable al gráfico BoxWhisker.

**Returns:**
int
### getShowConnectorLines() {#getShowConnectorLines--}
```
public boolean getShowConnectorLines()
```


Indica si se muestran líneas de conexión entre los puntos de datos.

**Remarks**

Solo para gráfico Waterfall.

**Returns:**
boolean
### getShowInnerPoints() {#getShowInnerPoints--}
```
public boolean getShowInnerPoints()
```


Indica si se muestran los puntos de datos que no son valores atípicos.

**Returns:**
boolean
### getShowMeanLine() {#getShowMeanLine--}
```
public boolean getShowMeanLine()
```


Indica si se muestra la línea que conecta todos los puntos de media.

**Remarks**

Solo funciona para el gráfico BoxWhisker.

**Returns:**
boolean
### getShowMeanMarker() {#getShowMeanMarker--}
```
public boolean getShowMeanMarker()
```


Indica si se muestran los marcadores que denotan la media.

**Returns:**
boolean
### getShowOutlierPoints() {#getShowOutlierPoints--}
```
public boolean getShowOutlierPoints()
```


Indica si se muestran los puntos de datos atípicos.

**Returns:**
boolean
### getSubtotals() {#getSubtotals--}
```
public int[] getSubtotals()
```


Representa el índice de un punto de datos subtotal.

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


Indica si el intervalo está cerrado en el lado izquierdo.

**Remarks**

Solo para gráfico ParetoLine.

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


Indica si el intervalo está cerrado en el lado izquierdo.

**Remarks**

Solo para gráfico ParetoLine.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setMapChartProjectionType(int value) {#setMapChartProjectionType-int-}
```
public void setMapChartProjectionType(int value)
```


Establece el tipo de proyección del mapa.

Ver [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Solo para gráfico de mapa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMapChartRegionType(int value) {#setMapChartRegionType-int-}
```
public void setMapChartRegionType(int value)
```


Establece el tipo de región del mapa.

Ver [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Solo para gráfico de mapa.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setMapLabelLayout(int value) {#setMapLabelLayout-int-}
```
public void setMapLabelLayout(int value)
```


Establece el diseño de las etiquetas del mapa.

Ver [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setQuartileCalculation(int value) {#setQuartileCalculation-int-}
```
public void setQuartileCalculation(int value)
```


Representa las propiedades estadísticas de la serie.

Ver [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Solo aplicable al gráfico BoxWhisker.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

### setShowConnectorLines(boolean value) {#setShowConnectorLines-boolean-}
```
public void setShowConnectorLines(boolean value)
```


Indica si se muestran líneas de conexión entre los puntos de datos.

**Remarks**

Solo para gráfico Waterfall.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowInnerPoints(boolean value) {#setShowInnerPoints-boolean-}
```
public void setShowInnerPoints(boolean value)
```


Indica si se muestran los puntos de datos que no son valores atípicos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowMeanLine(boolean value) {#setShowMeanLine-boolean-}
```
public void setShowMeanLine(boolean value)
```


Indica si se muestra la línea que conecta todos los puntos de media.

**Remarks**

Solo funciona para el gráfico BoxWhisker.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowMeanMarker(boolean value) {#setShowMeanMarker-boolean-}
```
public void setShowMeanMarker(boolean value)
```


Indica si se muestran los marcadores que denotan la media.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setShowOutlierPoints(boolean value) {#setShowOutlierPoints-boolean-}
```
public void setShowOutlierPoints(boolean value)
```


Indica si se muestran los puntos de datos atípicos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setSubtotals(int[] value) {#setSubtotals-int---}
```
public void setSubtotals(int[] value)
```


Representa el índice de un punto de datos subtotal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int[] |  |

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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

