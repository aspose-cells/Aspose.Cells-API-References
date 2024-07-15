---
title: SeriesLayoutProperties
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the properties of series layout.
type: docs
url: /nodejs-cpp/serieslayoutproperties/
---

## SeriesLayoutProperties class

Represents the properties of series layout.

```javascript
class SeriesLayoutProperties;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getShowConnectorLines()](#getShowConnectorLines--)| Indicates whether showing connector lines between data points. |
| [setShowConnectorLines(boolean)](#setShowConnectorLines-boolean-)| Indicates whether showing connector lines between data points. |
| [getShowMeanLine()](#getShowMeanLine--)| Indicates whether showing the line connecting all mean points. |
| [setShowMeanLine(boolean)](#setShowMeanLine-boolean-)| Indicates whether showing the line connecting all mean points. |
| [getShowOutlierPoints()](#getShowOutlierPoints--)| Indicates whether showing outlier data points. |
| [setShowOutlierPoints(boolean)](#setShowOutlierPoints-boolean-)| Indicates whether showing outlier data points. |
| [getShowMeanMarker()](#getShowMeanMarker--)| Indicates whether showing markers denoting the mean. |
| [setShowMeanMarker(boolean)](#setShowMeanMarker-boolean-)| Indicates whether showing markers denoting the mean. |
| [getShowInnerPoints()](#getShowInnerPoints--)| Indicates whether showing non-outlier data points. |
| [setShowInnerPoints(boolean)](#setShowInnerPoints-boolean-)| Indicates whether showing non-outlier data points. |
| [getSubtotals()](#getSubtotals--)| Represents the index of a subtotal data point. |
| [setSubtotals(number[])](#setSubtotals-numberarray-)| Represents the index of a subtotal data point. |
| [getQuartileCalculation()](#getQuartileCalculation--)| Represents the statistical properties for the series. |
| [setQuartileCalculation(QuartileCalculationType)](#setQuartileCalculation-quartilecalculationtype-)| Represents the statistical properties for the series. |
| [getMapLabelLayout()](#getMapLabelLayout--)| Gets and sets the layout of map labels. |
| [setMapLabelLayout(MapChartLabelLayout)](#setMapLabelLayout-mapchartlabellayout-)| Gets and sets the layout of map labels. |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--)| Indicates whether the interval is closed on the left side. |
| [setIsIntervalLeftClosed(boolean)](#setIsIntervalLeftClosed-boolean-)| Indicates whether the interval is closed on the left side. |
| [getMapChartRegionType()](#getMapChartRegionType--)| Gets and sets the region type of the map. |
| [setMapChartRegionType(MapChartRegionType)](#setMapChartRegionType-mapchartregiontype-)| Gets and sets the region type of the map. |
| [getMapChartProjectionType()](#getMapChartProjectionType--)| Gets and sets the projection type of the map. |
| [setMapChartProjectionType(MapChartProjectionType)](#setMapChartProjectionType-mapchartprojectiontype-)| Gets and sets the projection type of the map. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getShowConnectorLines() {#getShowConnectorLines--}

Indicates whether showing connector lines between data points.

```javascript
getShowConnectorLines() : boolean;
```


### setShowConnectorLines(boolean) {#setShowConnectorLines-boolean-}

Indicates whether showing connector lines between data points.

```javascript
setShowConnectorLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowMeanLine() {#getShowMeanLine--}

Indicates whether showing the line connecting all mean points.

```javascript
getShowMeanLine() : boolean;
```


### setShowMeanLine(boolean) {#setShowMeanLine-boolean-}

Indicates whether showing the line connecting all mean points.

```javascript
setShowMeanLine(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowOutlierPoints() {#getShowOutlierPoints--}

Indicates whether showing outlier data points.

```javascript
getShowOutlierPoints() : boolean;
```


### setShowOutlierPoints(boolean) {#setShowOutlierPoints-boolean-}

Indicates whether showing outlier data points.

```javascript
setShowOutlierPoints(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowMeanMarker() {#getShowMeanMarker--}

Indicates whether showing markers denoting the mean.

```javascript
getShowMeanMarker() : boolean;
```


### setShowMeanMarker(boolean) {#setShowMeanMarker-boolean-}

Indicates whether showing markers denoting the mean.

```javascript
setShowMeanMarker(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowInnerPoints() {#getShowInnerPoints--}

Indicates whether showing non-outlier data points.

```javascript
getShowInnerPoints() : boolean;
```


### setShowInnerPoints(boolean) {#setShowInnerPoints-boolean-}

Indicates whether showing non-outlier data points.

```javascript
setShowInnerPoints(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSubtotals() {#getSubtotals--}

Represents the index of a subtotal data point.

```javascript
getSubtotals() : number[];
```


**Returns**

number[]

### setSubtotals(number[]) {#setSubtotals-numberarray-}

Represents the index of a subtotal data point.

```javascript
setSubtotals(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getQuartileCalculation() {#getQuartileCalculation--}

Represents the statistical properties for the series.

```javascript
getQuartileCalculation() : QuartileCalculationType;
```


**Returns**

[QuartileCalculationType](../quartilecalculationtype/)

### setQuartileCalculation(QuartileCalculationType) {#setQuartileCalculation-quartilecalculationtype-}

Represents the statistical properties for the series.

```javascript
setQuartileCalculation(value: QuartileCalculationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [QuartileCalculationType](../quartilecalculationtype/) | The value to set. |

### getMapLabelLayout() {#getMapLabelLayout--}

Gets and sets the layout of map labels.

```javascript
getMapLabelLayout() : MapChartLabelLayout;
```


**Returns**

[MapChartLabelLayout](../mapchartlabellayout/)

### setMapLabelLayout(MapChartLabelLayout) {#setMapLabelLayout-mapchartlabellayout-}

Gets and sets the layout of map labels.

```javascript
setMapLabelLayout(value: MapChartLabelLayout) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartLabelLayout](../mapchartlabellayout/) | The value to set. |

### isIntervalLeftClosed() {#isIntervalLeftClosed--}

Indicates whether the interval is closed on the left side.

```javascript
isIntervalLeftClosed() : boolean;
```


### setIsIntervalLeftClosed(boolean) {#setIsIntervalLeftClosed-boolean-}

Indicates whether the interval is closed on the left side.

```javascript
setIsIntervalLeftClosed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMapChartRegionType() {#getMapChartRegionType--}

Gets and sets the region type of the map.

```javascript
getMapChartRegionType() : MapChartRegionType;
```


**Returns**

[MapChartRegionType](../mapchartregiontype/)

### setMapChartRegionType(MapChartRegionType) {#setMapChartRegionType-mapchartregiontype-}

Gets and sets the region type of the map.

```javascript
setMapChartRegionType(value: MapChartRegionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartRegionType](../mapchartregiontype/) | The value to set. |

### getMapChartProjectionType() {#getMapChartProjectionType--}

Gets and sets the projection type of the map.

```javascript
getMapChartProjectionType() : MapChartProjectionType;
```


**Returns**

[MapChartProjectionType](../mapchartprojectiontype/)

### setMapChartProjectionType(MapChartProjectionType) {#setMapChartProjectionType-mapchartprojectiontype-}

Gets and sets the projection type of the map.

```javascript
setMapChartProjectionType(value: MapChartProjectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartProjectionType](../mapchartprojectiontype/) | The value to set. |


