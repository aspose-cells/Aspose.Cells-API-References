---
title: "SeriesLayoutProperties"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет свойства макета серии."
type: docs
url: /ru/java/com.aspose.cells/serieslayoutproperties/
---

**Inheritance:**
java.lang.Object
```
public class SeriesLayoutProperties
```

Представляет свойства макета серии.

**Remarks**

Применяется только к диаграммам BoxWhisker, Funnel, ParetoLine, Sunburst, Treemap, Waterfall и Histogram.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SeriesLayoutProperties()](#SeriesLayoutProperties--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMapChartProjectionType()](#getMapChartProjectionType--) | Получает тип проекции карты. |
| [getMapChartRegionType()](#getMapChartRegionType--) | Получает тип региона карты. |
| [getMapLabelLayout()](#getMapLabelLayout--) | Получает расположение меток карты. |
| [getQuartileCalculation()](#getQuartileCalculation--) | Представляет статистические свойства для серии. |
| [getShowConnectorLines()](#getShowConnectorLines--) | Указывает, отображаются ли соединительные линии между точками данных. |
| [getShowInnerPoints()](#getShowInnerPoints--) | Указывает, показывать ли точки данных, не являющиеся выбросами. |
| [getShowMeanLine()](#getShowMeanLine--) | Указывает, показывать ли линию, соединяющую все точки среднего значения. |
| [getShowMeanMarker()](#getShowMeanMarker--) | Указывает, отображаются ли маркеры, обозначающие среднее. |
| [getShowOutlierPoints()](#getShowOutlierPoints--) | Указывает, отображаются ли точки данных‑выбросы. |
| [getSubtotals()](#getSubtotals--) | Представляет индекс точки данных подытога. |
| [hashCode()](#hashCode--) |  |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--) | Указывает, закрыт ли интервал слева. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setIntervalLeftClosed(boolean value)](#setIntervalLeftClosed-boolean-) | Указывает, закрыт ли интервал слева. |
| [setMapChartProjectionType(int value)](#setMapChartProjectionType-int-) | Устанавливает тип проекции карты. |
| [setMapChartRegionType(int value)](#setMapChartRegionType-int-) | Устанавливает тип региона карты. |
| [setMapLabelLayout(int value)](#setMapLabelLayout-int-) | Устанавливает расположение меток карты. |
| [setQuartileCalculation(int value)](#setQuartileCalculation-int-) | Представляет статистические свойства для серии. |
| [setShowConnectorLines(boolean value)](#setShowConnectorLines-boolean-) | Указывает, отображаются ли соединительные линии между точками данных. |
| [setShowInnerPoints(boolean value)](#setShowInnerPoints-boolean-) | Указывает, показывать ли точки данных, не являющиеся выбросами. |
| [setShowMeanLine(boolean value)](#setShowMeanLine-boolean-) | Указывает, показывать ли линию, соединяющую все точки среднего значения. |
| [setShowMeanMarker(boolean value)](#setShowMeanMarker-boolean-) | Указывает, отображаются ли маркеры, обозначающие среднее. |
| [setShowOutlierPoints(boolean value)](#setShowOutlierPoints-boolean-) | Указывает, отображаются ли точки данных‑выбросы. |
| [setSubtotals(int[] value)](#setSubtotals-int---) | Представляет индекс точки данных подытога. |
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
| Параметр | Тип | Описание |
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


Получает тип проекции карты.

См. [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Только для картовой диаграммы.

**Returns:**
int
### getMapChartRegionType() {#getMapChartRegionType--}
```
public int getMapChartRegionType()
```


Получает тип региона карты.

См. [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Только для картовой диаграммы.

**Returns:**
int
### getMapLabelLayout() {#getMapLabelLayout--}
```
public int getMapLabelLayout()
```


Получает расположение меток карты.

См. [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Returns:**
int
### getQuartileCalculation() {#getQuartileCalculation--}
```
public int getQuartileCalculation()
```


Представляет статистические свойства для серии.

См. [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Только применимо к диаграмме BoxWhisker.

**Returns:**
int
### getShowConnectorLines() {#getShowConnectorLines--}
```
public boolean getShowConnectorLines()
```


Указывает, отображаются ли соединительные линии между точками данных.

**Remarks**

Только для диаграммы Waterfall.

**Returns:**
boolean
### getShowInnerPoints() {#getShowInnerPoints--}
```
public boolean getShowInnerPoints()
```


Указывает, показывать ли точки данных, не являющиеся выбросами.

**Returns:**
boolean
### getShowMeanLine() {#getShowMeanLine--}
```
public boolean getShowMeanLine()
```


Указывает, показывать ли линию, соединяющую все точки среднего значения.

**Remarks**

Работает только с диаграммой BoxWhisker.

**Returns:**
boolean
### getShowMeanMarker() {#getShowMeanMarker--}
```
public boolean getShowMeanMarker()
```


Указывает, отображаются ли маркеры, обозначающие среднее.

**Returns:**
boolean
### getShowOutlierPoints() {#getShowOutlierPoints--}
```
public boolean getShowOutlierPoints()
```


Указывает, отображаются ли точки данных‑выбросы.

**Returns:**
boolean
### getSubtotals() {#getSubtotals--}
```
public int[] getSubtotals()
```


Представляет индекс точки данных подытога.

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


Указывает, закрыт ли интервал слева.

**Remarks**

Только для диаграммы ParetoLine.

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


Указывает, закрыт ли интервал слева.

**Remarks**

Только для диаграммы ParetoLine.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setMapChartProjectionType(int value) {#setMapChartProjectionType-int-}
```
public void setMapChartProjectionType(int value)
```


Устанавливает тип проекции карты.

См. [MapChartProjectionType](../../com.aspose.cells/mapchartprojectiontype).

**Remarks**

Только для картовой диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMapChartRegionType(int value) {#setMapChartRegionType-int-}
```
public void setMapChartRegionType(int value)
```


Устанавливает тип региона карты.

См. [MapChartRegionType](../../com.aspose.cells/mapchartregiontype).

**Remarks**

Только для картовой диаграммы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setMapLabelLayout(int value) {#setMapLabelLayout-int-}
```
public void setMapLabelLayout(int value)
```


Устанавливает расположение меток карты.

См. [MapChartLabelLayout](../../com.aspose.cells/mapchartlabellayout).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setQuartileCalculation(int value) {#setQuartileCalculation-int-}
```
public void setQuartileCalculation(int value)
```


Представляет статистические свойства для серии.

См. [QuartileCalculationType](../../com.aspose.cells/quartilecalculationtype).

**Remarks**

Только применимо к диаграмме BoxWhisker.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

### setShowConnectorLines(boolean value) {#setShowConnectorLines-boolean-}
```
public void setShowConnectorLines(boolean value)
```


Указывает, отображаются ли соединительные линии между точками данных.

**Remarks**

Только для диаграммы Waterfall.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowInnerPoints(boolean value) {#setShowInnerPoints-boolean-}
```
public void setShowInnerPoints(boolean value)
```


Указывает, показывать ли точки данных, не являющиеся выбросами.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowMeanLine(boolean value) {#setShowMeanLine-boolean-}
```
public void setShowMeanLine(boolean value)
```


Указывает, показывать ли линию, соединяющую все точки среднего значения.

**Remarks**

Работает только с диаграммой BoxWhisker.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowMeanMarker(boolean value) {#setShowMeanMarker-boolean-}
```
public void setShowMeanMarker(boolean value)
```


Указывает, отображаются ли маркеры, обозначающие среднее.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setShowOutlierPoints(boolean value) {#setShowOutlierPoints-boolean-}
```
public void setShowOutlierPoints(boolean value)
```


Указывает, отображаются ли точки данных‑выбросы.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean |  |

### setSubtotals(int[] value) {#setSubtotals-int---}
```
public void setSubtotals(int[] value)
```


Представляет индекс точки данных подытога.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int[] |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

