---
title: "SeriesLayoutProperties"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Eigenschaften des Serienlayouts dar."
type: docs
url: /de/java/com.aspose.cells/serieslayoutproperties/
---

**Inheritance:**
java.lang.Object
```
public class SeriesLayoutProperties
```

Stellt die Eigenschaften des Serienlayouts dar.

**Remarks**

Nur anwendbar auf die Diagramme BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall und Histogram.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SeriesLayoutProperties()](#SeriesLayoutProperties--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMapChartProjectionType()](#getMapChartProjectionType--) | Liefert den Projektionstyp der Karte. |
| [getMapChartRegionType()](#getMapChartRegionType--) | Liefert den Regionstyp der Karte. |
| [getMapLabelLayout()](#getMapLabelLayout--) | Liefert das Layout der Kartenbeschriftungen. |
| [getQuartileCalculation()](#getQuartileCalculation--) | Stellt die statistischen Eigenschaften für die Serie dar. |
| [getShowConnectorLines()](#getShowConnectorLines--) | Gibt an, ob Verbindungslinien zwischen Datenpunkten angezeigt werden. |
| [getShowInnerPoints()](#getShowInnerPoints--) | Gibt an, ob Nicht‑Ausreißer‑Datenpunkte angezeigt werden sollen. |
| [getShowMeanLine()](#getShowMeanLine--) | Gibt an, ob die Linie angezeigt werden soll, die alle Mittelwertpunkte verbindet. |
| [getShowMeanMarker()](#getShowMeanMarker--) | Gibt an, ob Markierungen, die den Mittelwert bezeichnen, angezeigt werden. |
| [getShowOutlierPoints()](#getShowOutlierPoints--) | Gibt an, ob Ausreißer‑Datenpunkte angezeigt werden. |
| [getSubtotals()](#getSubtotals--) | Stellt den Index eines Zwischensummen‑Datenpunkts dar. |
| [hashCode()](#hashCode--) |  |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--) | Gibt an, ob das Intervall auf der linken Seite geschlossen ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIntervalLeftClosed(boolean value)](#setIntervalLeftClosed-boolean-) | Gibt an, ob das Intervall auf der linken Seite geschlossen ist. |
| [setMapChartProjectionType(int value)](#setMapChartProjectionType-int-) | Legt den Projektionstyp der Karte fest. |
| [setMapChartRegionType(int value)](#setMapChartRegionType-int-) | Legt den Regionstyp der Karte fest. |
| [setMapLabelLayout(int value)](#setMapLabelLayout-int-) | Legt das Layout der Kartenbeschriftungen fest. |
| [setQuartileCalculation(int value)](#setQuartileCalculation-int-) | Stellt die statistischen Eigenschaften für die Serie dar. |
| [setShowConnectorLines(boolean value)](#setShowConnectorLines-boolean-) | Gibt an, ob Verbindungslinien zwischen Datenpunkten angezeigt werden. |
| [setShowInnerPoints(boolean value)](#setShowInnerPoints-boolean-) | Gibt an, ob Nicht‑Ausreißer‑Datenpunkte angezeigt werden sollen. |
| [setShowMeanLine(boolean value)](#setShowMeanLine-boolean-) | Gibt an, ob die Linie angezeigt werden soll, die alle Mittelwertpunkte verbindet. |
| [setShowMeanMarker(boolean value)](#setShowMeanMarker-boolean-) | Gibt an, ob Markierungen, die den Mittelwert bezeichnen, angezeigt werden. |
| [setShowOutlierPoints(boolean value)](#setShowOutlierPoints-boolean-) | Gibt an, ob Ausreißer‑Datenpunkte angezeigt werden. |
| [setSubtotals(int[] value)](#setSubtotals-int---) | Stellt den Index eines Zwischensummen‑Datenpunkts dar. |
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
| Parameter | Typ | Beschreibung |
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


Liefert den Projektionstyp der Karte.

Siehe [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Nur für Karten‑Diagramm.

**Returns:**
int
### getMapChartRegionType() {#getMapChartRegionType--}
```
public int getMapChartRegionType()
```


Liefert den Regionstyp der Karte.

Siehe [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Nur für Karten‑Diagramm.

**Returns:**
int
### getMapLabelLayout() {#getMapLabelLayout--}
```
public int getMapLabelLayout()
```


Liefert das Layout der Kartenbeschriftungen.

Siehe [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Returns:**
int
### getQuartileCalculation() {#getQuartileCalculation--}
```
public int getQuartileCalculation()
```


Stellt die statistischen Eigenschaften für die Serie dar.

Siehe [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Nur anwendbar auf BoxWhisker‑Diagramm.

**Returns:**
int
### getShowConnectorLines() {#getShowConnectorLines--}
```
public boolean getShowConnectorLines()
```


Gibt an, ob Verbindungslinien zwischen Datenpunkten angezeigt werden.

**Remarks**

Nur für Wasserfall‑Diagramm.

**Returns:**
boolean
### getShowInnerPoints() {#getShowInnerPoints--}
```
public boolean getShowInnerPoints()
```


Gibt an, ob Nicht‑Ausreißer‑Datenpunkte angezeigt werden sollen.

**Returns:**
boolean
### getShowMeanLine() {#getShowMeanLine--}
```
public boolean getShowMeanLine()
```


Gibt an, ob die Linie angezeigt werden soll, die alle Mittelwertpunkte verbindet.

**Remarks**

Funktioniert nur für BoxWhisker‑Diagramm.

**Returns:**
boolean
### getShowMeanMarker() {#getShowMeanMarker--}
```
public boolean getShowMeanMarker()
```


Gibt an, ob Markierungen, die den Mittelwert bezeichnen, angezeigt werden.

**Returns:**
boolean
### getShowOutlierPoints() {#getShowOutlierPoints--}
```
public boolean getShowOutlierPoints()
```


Gibt an, ob Ausreißer‑Datenpunkte angezeigt werden.

**Returns:**
boolean
### getSubtotals() {#getSubtotals--}
```
public int[] getSubtotals()
```


Stellt den Index eines Zwischensummen‑Datenpunkts dar.

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


Gibt an, ob das Intervall auf der linken Seite geschlossen ist.

**Remarks**

Nur für ParetoLine‑Diagramm.

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


Gibt an, ob das Intervall auf der linken Seite geschlossen ist.

**Remarks**

Nur für ParetoLine‑Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMapChartProjectionType(int value) {#setMapChartProjectionType-int-}
```
public void setMapChartProjectionType(int value)
```


Legt den Projektionstyp der Karte fest.

Siehe [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Nur für Karten‑Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMapChartRegionType(int value) {#setMapChartRegionType-int-}
```
public void setMapChartRegionType(int value)
```


Legt den Regionstyp der Karte fest.

Siehe [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Nur für Karten‑Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMapLabelLayout(int value) {#setMapLabelLayout-int-}
```
public void setMapLabelLayout(int value)
```


Legt das Layout der Kartenbeschriftungen fest.

Siehe [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setQuartileCalculation(int value) {#setQuartileCalculation-int-}
```
public void setQuartileCalculation(int value)
```


Stellt die statistischen Eigenschaften für die Serie dar.

Siehe [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Nur anwendbar auf BoxWhisker‑Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShowConnectorLines(boolean value) {#setShowConnectorLines-boolean-}
```
public void setShowConnectorLines(boolean value)
```


Gibt an, ob Verbindungslinien zwischen Datenpunkten angezeigt werden.

**Remarks**

Nur für Wasserfall‑Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowInnerPoints(boolean value) {#setShowInnerPoints-boolean-}
```
public void setShowInnerPoints(boolean value)
```


Gibt an, ob Nicht‑Ausreißer‑Datenpunkte angezeigt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowMeanLine(boolean value) {#setShowMeanLine-boolean-}
```
public void setShowMeanLine(boolean value)
```


Gibt an, ob die Linie angezeigt werden soll, die alle Mittelwertpunkte verbindet.

**Remarks**

Funktioniert nur für BoxWhisker‑Diagramm.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowMeanMarker(boolean value) {#setShowMeanMarker-boolean-}
```
public void setShowMeanMarker(boolean value)
```


Gibt an, ob Markierungen, die den Mittelwert bezeichnen, angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowOutlierPoints(boolean value) {#setShowOutlierPoints-boolean-}
```
public void setShowOutlierPoints(boolean value)
```


Gibt an, ob Ausreißer‑Datenpunkte angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSubtotals(int[] value) {#setSubtotals-int---}
```
public void setSubtotals(int[] value)
```


Stellt den Index eines Zwischensummen‑Datenpunkts dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int[] |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

