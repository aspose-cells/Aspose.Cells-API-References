---
title: "SeriesLayoutProperties"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar egenskaperna för serielayouten."
type: docs
url: /sv/java/com.aspose.cells/serieslayoutproperties/
---

**Inheritance:**
java.lang.Object
```
public class SeriesLayoutProperties
```

Representerar egenskaperna för serielayouten.

**Remarks**

Endast tillämplig på diagrammen BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall och Histogram.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SeriesLayoutProperties()](#SeriesLayoutProperties--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMapChartProjectionType()](#getMapChartProjectionType--) | Hämtar projektionstypen för kartan. |
| [getMapChartRegionType()](#getMapChartRegionType--) | Hämtar regionstypen för kartan. |
| [getMapLabelLayout()](#getMapLabelLayout--) | Hämtar layouten för kartetiketter. |
| [getQuartileCalculation()](#getQuartileCalculation--) | Representerar de statistiska egenskaperna för serien. |
| [getShowConnectorLines()](#getShowConnectorLines--) | Indikerar om anslutningslinjer visas mellan datapunkter. |
| [getShowInnerPoints()](#getShowInnerPoints--) | Indikerar om icke-avvikande datapunkter ska visas. |
| [getShowMeanLine()](#getShowMeanLine--) | Indikerar om linjen som förbinder alla medelvärdespunkter. |
| [getShowMeanMarker()](#getShowMeanMarker--) | Indikerar om markörer som anger medelvärdet visas. |
| [getShowOutlierPoints()](#getShowOutlierPoints--) | Indikerar om avvikande datapunkter visas. |
| [getSubtotals()](#getSubtotals--) | Representerar indexet för en delsumme-datapunkt. |
| [hashCode()](#hashCode--) |  |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--) | Indikerar om intervallet är stängt på vänstra sidan. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIntervalLeftClosed(boolean value)](#setIntervalLeftClosed-boolean-) | Indikerar om intervallet är stängt på vänstra sidan. |
| [setMapChartProjectionType(int value)](#setMapChartProjectionType-int-) | Ställer in projektionstypen för kartan. |
| [setMapChartRegionType(int value)](#setMapChartRegionType-int-) | Ställer in regionstypen för kartan. |
| [setMapLabelLayout(int value)](#setMapLabelLayout-int-) | Ställer in layouten för kartetiketter. |
| [setQuartileCalculation(int value)](#setQuartileCalculation-int-) | Representerar de statistiska egenskaperna för serien. |
| [setShowConnectorLines(boolean value)](#setShowConnectorLines-boolean-) | Indikerar om anslutningslinjer visas mellan datapunkter. |
| [setShowInnerPoints(boolean value)](#setShowInnerPoints-boolean-) | Indikerar om icke-avvikande datapunkter ska visas. |
| [setShowMeanLine(boolean value)](#setShowMeanLine-boolean-) | Indikerar om linjen som förbinder alla medelvärdespunkter. |
| [setShowMeanMarker(boolean value)](#setShowMeanMarker-boolean-) | Indikerar om markörer som anger medelvärdet visas. |
| [setShowOutlierPoints(boolean value)](#setShowOutlierPoints-boolean-) | Indikerar om avvikande datapunkter visas. |
| [setSubtotals(int[] value)](#setSubtotals-int---) | Representerar indexet för en delsumme-datapunkt. |
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
| Parameter | Typ | Beskrivning |
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


Hämtar projektionstypen för kartan.

Se [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Endast för kartdiagram.

**Returns:**
int
### getMapChartRegionType() {#getMapChartRegionType--}
```
public int getMapChartRegionType()
```


Hämtar regionstypen för kartan.

Se [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Endast för kartdiagram.

**Returns:**
int
### getMapLabelLayout() {#getMapLabelLayout--}
```
public int getMapLabelLayout()
```


Hämtar layouten för kartetiketter.

Se [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Returns:**
int
### getQuartileCalculation() {#getQuartileCalculation--}
```
public int getQuartileCalculation()
```


Representerar de statistiska egenskaperna för serien.

Se [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Endast tillämplig på BoxWhisker-diagram.

**Returns:**
int
### getShowConnectorLines() {#getShowConnectorLines--}
```
public boolean getShowConnectorLines()
```


Indikerar om anslutningslinjer visas mellan datapunkter.

**Remarks**

Endast för Waterfall-diagram.

**Returns:**
boolean
### getShowInnerPoints() {#getShowInnerPoints--}
```
public boolean getShowInnerPoints()
```


Indikerar om icke-avvikande datapunkter ska visas.

**Returns:**
boolean
### getShowMeanLine() {#getShowMeanLine--}
```
public boolean getShowMeanLine()
```


Indikerar om linjen som förbinder alla medelvärdespunkter.

**Remarks**

Fungerar endast för BoxWhisker-diagram.

**Returns:**
boolean
### getShowMeanMarker() {#getShowMeanMarker--}
```
public boolean getShowMeanMarker()
```


Indikerar om markörer som anger medelvärdet visas.

**Returns:**
boolean
### getShowOutlierPoints() {#getShowOutlierPoints--}
```
public boolean getShowOutlierPoints()
```


Indikerar om avvikande datapunkter visas.

**Returns:**
boolean
### getSubtotals() {#getSubtotals--}
```
public int[] getSubtotals()
```


Representerar indexet för en delsumme-datapunkt.

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


Indikerar om intervallet är stängt på vänstra sidan.

**Remarks**

Endast för ParetoLine-diagram.

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


Indikerar om intervallet är stängt på vänstra sidan.

**Remarks**

Endast för ParetoLine-diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMapChartProjectionType(int value) {#setMapChartProjectionType-int-}
```
public void setMapChartProjectionType(int value)
```


Ställer in projektionstypen för kartan.

Se [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Endast för kartdiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMapChartRegionType(int value) {#setMapChartRegionType-int-}
```
public void setMapChartRegionType(int value)
```


Ställer in regionstypen för kartan.

Se [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Endast för kartdiagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMapLabelLayout(int value) {#setMapLabelLayout-int-}
```
public void setMapLabelLayout(int value)
```


Ställer in layouten för kartetiketter.

Se [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setQuartileCalculation(int value) {#setQuartileCalculation-int-}
```
public void setQuartileCalculation(int value)
```


Representerar de statistiska egenskaperna för serien.

Se [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Endast tillämplig på BoxWhisker-diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowConnectorLines(boolean value) {#setShowConnectorLines-boolean-}
```
public void setShowConnectorLines(boolean value)
```


Indikerar om anslutningslinjer visas mellan datapunkter.

**Remarks**

Endast för Waterfall-diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowInnerPoints(boolean value) {#setShowInnerPoints-boolean-}
```
public void setShowInnerPoints(boolean value)
```


Indikerar om icke-avvikande datapunkter ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowMeanLine(boolean value) {#setShowMeanLine-boolean-}
```
public void setShowMeanLine(boolean value)
```


Indikerar om linjen som förbinder alla medelvärdespunkter.

**Remarks**

Fungerar endast för BoxWhisker-diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowMeanMarker(boolean value) {#setShowMeanMarker-boolean-}
```
public void setShowMeanMarker(boolean value)
```


Indikerar om markörer som anger medelvärdet visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowOutlierPoints(boolean value) {#setShowOutlierPoints-boolean-}
```
public void setShowOutlierPoints(boolean value)
```


Indikerar om avvikande datapunkter visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSubtotals(int[] value) {#setSubtotals-int---}
```
public void setSubtotals(int[] value)
```


Representerar indexet för en delsumme-datapunkt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int[] |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

