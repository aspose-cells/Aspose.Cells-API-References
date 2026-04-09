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

### Remarks
Only applicable to BoxWhisker,Funnel,ParetoLine,Sunburst,Treemap,Waterfall and Histogram chart.

## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [showConnectorLines](#showConnectorLines--)| boolean | Indicates whether connector lines are shown between data points. |
| [showMeanLine](#showMeanLine--)| boolean | Indicates whether to show the line connecting all mean points. |
| [showOutlierPoints](#showOutlierPoints--)| boolean | Indicates whether outlier data points are shown. |
| [showMeanMarker](#showMeanMarker--)| boolean | Indicates whether markers denoting the mean are shown. |
| [showInnerPoints](#showInnerPoints--)| boolean | Indicates whether to show non-outlier data points. |
| [subtotals](#subtotals--)| number[] | Represents the index of a subtotal data point. |
| [quartileCalculation](#quartileCalculation--)| QuartileCalculationType | Represents the statistical properties for the series. |
| [mapLabelLayout](#mapLabelLayout--)| MapChartLabelLayout | Gets and sets the layout of map labels. |
| [isIntervalLeftClosed](#isIntervalLeftClosed--)| boolean | Indicates whether the interval is closed on the left side. |
| [mapChartRegionType](#mapChartRegionType--)| MapChartRegionType | Gets and sets the region type of the map. |
| [mapChartProjectionType](#mapChartProjectionType--)| MapChartProjectionType | Gets and sets the projection type of the map. |

## Methods

| Method | Description |
| --- | --- |
| [getShowConnectorLines()](#getShowConnectorLines--)| <b>@deprecated.</b> Please use the 'showConnectorLines' property instead. Indicates whether connector lines are shown between data points. |
| [setShowConnectorLines(boolean)](#setShowConnectorLines-boolean-)| <b>@deprecated.</b> Please use the 'showConnectorLines' property instead. Indicates whether connector lines are shown between data points. |
| [getShowMeanLine()](#getShowMeanLine--)| <b>@deprecated.</b> Please use the 'showMeanLine' property instead. Indicates whether to show the line connecting all mean points. |
| [setShowMeanLine(boolean)](#setShowMeanLine-boolean-)| <b>@deprecated.</b> Please use the 'showMeanLine' property instead. Indicates whether to show the line connecting all mean points. |
| [getShowOutlierPoints()](#getShowOutlierPoints--)| <b>@deprecated.</b> Please use the 'showOutlierPoints' property instead. Indicates whether outlier data points are shown. |
| [setShowOutlierPoints(boolean)](#setShowOutlierPoints-boolean-)| <b>@deprecated.</b> Please use the 'showOutlierPoints' property instead. Indicates whether outlier data points are shown. |
| [getShowMeanMarker()](#getShowMeanMarker--)| <b>@deprecated.</b> Please use the 'showMeanMarker' property instead. Indicates whether markers denoting the mean are shown. |
| [setShowMeanMarker(boolean)](#setShowMeanMarker-boolean-)| <b>@deprecated.</b> Please use the 'showMeanMarker' property instead. Indicates whether markers denoting the mean are shown. |
| [getShowInnerPoints()](#getShowInnerPoints--)| <b>@deprecated.</b> Please use the 'showInnerPoints' property instead. Indicates whether to show non-outlier data points. |
| [setShowInnerPoints(boolean)](#setShowInnerPoints-boolean-)| <b>@deprecated.</b> Please use the 'showInnerPoints' property instead. Indicates whether to show non-outlier data points. |
| [getSubtotals()](#getSubtotals--)| <b>@deprecated.</b> Please use the 'subtotals' property instead. Represents the index of a subtotal data point. |
| [setSubtotals(number[])](#setSubtotals-numberarray-)| <b>@deprecated.</b> Please use the 'subtotals' property instead. Represents the index of a subtotal data point. |
| [getQuartileCalculation()](#getQuartileCalculation--)| <b>@deprecated.</b> Please use the 'quartileCalculation' property instead. Represents the statistical properties for the series. |
| [setQuartileCalculation(QuartileCalculationType)](#setQuartileCalculation-quartilecalculationtype-)| <b>@deprecated.</b> Please use the 'quartileCalculation' property instead. Represents the statistical properties for the series. |
| [getMapLabelLayout()](#getMapLabelLayout--)| <b>@deprecated.</b> Please use the 'mapLabelLayout' property instead. Gets and sets the layout of map labels. |
| [setMapLabelLayout(MapChartLabelLayout)](#setMapLabelLayout-mapchartlabellayout-)| <b>@deprecated.</b> Please use the 'mapLabelLayout' property instead. Gets and sets the layout of map labels. |
| [isIntervalLeftClosed()](#isIntervalLeftClosed--)| <b>@deprecated.</b> Please use the 'isIntervalLeftClosed' property instead. Indicates whether the interval is closed on the left side. |
| [setIsIntervalLeftClosed(boolean)](#setIsIntervalLeftClosed-boolean-)| <b>@deprecated.</b> Please use the 'isIntervalLeftClosed' property instead. Indicates whether the interval is closed on the left side. |
| [getMapChartRegionType()](#getMapChartRegionType--)| <b>@deprecated.</b> Please use the 'mapChartRegionType' property instead. Gets and sets the region type of the map. |
| [setMapChartRegionType(MapChartRegionType)](#setMapChartRegionType-mapchartregiontype-)| <b>@deprecated.</b> Please use the 'mapChartRegionType' property instead. Gets and sets the region type of the map. |
| [getMapChartProjectionType()](#getMapChartProjectionType--)| <b>@deprecated.</b> Please use the 'mapChartProjectionType' property instead. Gets and sets the projection type of the map. |
| [setMapChartProjectionType(MapChartProjectionType)](#setMapChartProjectionType-mapchartprojectiontype-)| <b>@deprecated.</b> Please use the 'mapChartProjectionType' property instead. Gets and sets the projection type of the map. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### showConnectorLines {#showConnectorLines--}

Indicates whether connector lines are shown between data points.

```javascript
showConnectorLines : boolean;
```


**Remarks**

Only for Waterfall chart.

### showMeanLine {#showMeanLine--}

Indicates whether to show the line connecting all mean points.

```javascript
showMeanLine : boolean;
```


**Remarks**

Only works for BoxWhisker chart.

### showOutlierPoints {#showOutlierPoints--}

Indicates whether outlier data points are shown.

```javascript
showOutlierPoints : boolean;
```


### showMeanMarker {#showMeanMarker--}

Indicates whether markers denoting the mean are shown.

```javascript
showMeanMarker : boolean;
```


### showInnerPoints {#showInnerPoints--}

Indicates whether to show non-outlier data points.

```javascript
showInnerPoints : boolean;
```


### subtotals {#subtotals--}

Represents the index of a subtotal data point.

```javascript
subtotals : number[];
```


### quartileCalculation {#quartileCalculation--}

Represents the statistical properties for the series.

```javascript
quartileCalculation : QuartileCalculationType;
```


**Remarks**

Only applicable to BoxWhisker chart.

### mapLabelLayout {#mapLabelLayout--}

Gets and sets the layout of map labels.

```javascript
mapLabelLayout : MapChartLabelLayout;
```


### isIntervalLeftClosed {#isIntervalLeftClosed--}

Indicates whether the interval is closed on the left side.

```javascript
isIntervalLeftClosed : boolean;
```


**Remarks**

Only for ParetoLine chart.

### mapChartRegionType {#mapChartRegionType--}

Gets and sets the region type of the map.

```javascript
mapChartRegionType : MapChartRegionType;
```


**Remarks**

Only for map chart.

### mapChartProjectionType {#mapChartProjectionType--}

Gets and sets the projection type of the map.

```javascript
mapChartProjectionType : MapChartProjectionType;
```


**Remarks**

Only for map chart.

### getShowConnectorLines() {#getShowConnectorLines--}

<b>@deprecated.</b> Please use the 'showConnectorLines' property instead. Indicates whether connector lines are shown between data points.

```javascript
getShowConnectorLines() : boolean;
```


**Remarks**

Only for Waterfall chart.

### setShowConnectorLines(boolean) {#setShowConnectorLines-boolean-}

<b>@deprecated.</b> Please use the 'showConnectorLines' property instead. Indicates whether connector lines are shown between data points.

```javascript
setShowConnectorLines(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for Waterfall chart.

### getShowMeanLine() {#getShowMeanLine--}

<b>@deprecated.</b> Please use the 'showMeanLine' property instead. Indicates whether to show the line connecting all mean points.

```javascript
getShowMeanLine() : boolean;
```


**Remarks**

Only works for BoxWhisker chart.

### setShowMeanLine(boolean) {#setShowMeanLine-boolean-}

<b>@deprecated.</b> Please use the 'showMeanLine' property instead. Indicates whether to show the line connecting all mean points.

```javascript
setShowMeanLine(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works for BoxWhisker chart.

### getShowOutlierPoints() {#getShowOutlierPoints--}

<b>@deprecated.</b> Please use the 'showOutlierPoints' property instead. Indicates whether outlier data points are shown.

```javascript
getShowOutlierPoints() : boolean;
```


### setShowOutlierPoints(boolean) {#setShowOutlierPoints-boolean-}

<b>@deprecated.</b> Please use the 'showOutlierPoints' property instead. Indicates whether outlier data points are shown.

```javascript
setShowOutlierPoints(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowMeanMarker() {#getShowMeanMarker--}

<b>@deprecated.</b> Please use the 'showMeanMarker' property instead. Indicates whether markers denoting the mean are shown.

```javascript
getShowMeanMarker() : boolean;
```


### setShowMeanMarker(boolean) {#setShowMeanMarker-boolean-}

<b>@deprecated.</b> Please use the 'showMeanMarker' property instead. Indicates whether markers denoting the mean are shown.

```javascript
setShowMeanMarker(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowInnerPoints() {#getShowInnerPoints--}

<b>@deprecated.</b> Please use the 'showInnerPoints' property instead. Indicates whether to show non-outlier data points.

```javascript
getShowInnerPoints() : boolean;
```


### setShowInnerPoints(boolean) {#setShowInnerPoints-boolean-}

<b>@deprecated.</b> Please use the 'showInnerPoints' property instead. Indicates whether to show non-outlier data points.

```javascript
setShowInnerPoints(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSubtotals() {#getSubtotals--}

<b>@deprecated.</b> Please use the 'subtotals' property instead. Represents the index of a subtotal data point.

```javascript
getSubtotals() : number[];
```


**Returns**

number[]

### setSubtotals(number[]) {#setSubtotals-numberarray-}

<b>@deprecated.</b> Please use the 'subtotals' property instead. Represents the index of a subtotal data point.

```javascript
setSubtotals(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getQuartileCalculation() {#getQuartileCalculation--}

<b>@deprecated.</b> Please use the 'quartileCalculation' property instead. Represents the statistical properties for the series.

```javascript
getQuartileCalculation() : QuartileCalculationType;
```


**Returns**

[QuartileCalculationType](../quartilecalculationtype/)

**Remarks**

Only applicable to BoxWhisker chart.

### setQuartileCalculation(QuartileCalculationType) {#setQuartileCalculation-quartilecalculationtype-}

<b>@deprecated.</b> Please use the 'quartileCalculation' property instead. Represents the statistical properties for the series.

```javascript
setQuartileCalculation(value: QuartileCalculationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [QuartileCalculationType](../quartilecalculationtype/) | The value to set. |

**Remarks**

Only applicable to BoxWhisker chart.

### getMapLabelLayout() {#getMapLabelLayout--}

<b>@deprecated.</b> Please use the 'mapLabelLayout' property instead. Gets and sets the layout of map labels.

```javascript
getMapLabelLayout() : MapChartLabelLayout;
```


**Returns**

[MapChartLabelLayout](../mapchartlabellayout/)

### setMapLabelLayout(MapChartLabelLayout) {#setMapLabelLayout-mapchartlabellayout-}

<b>@deprecated.</b> Please use the 'mapLabelLayout' property instead. Gets and sets the layout of map labels.

```javascript
setMapLabelLayout(value: MapChartLabelLayout) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartLabelLayout](../mapchartlabellayout/) | The value to set. |

### isIntervalLeftClosed() {#isIntervalLeftClosed--}

<b>@deprecated.</b> Please use the 'isIntervalLeftClosed' property instead. Indicates whether the interval is closed on the left side.

```javascript
isIntervalLeftClosed() : boolean;
```


**Remarks**

Only for ParetoLine chart.

### setIsIntervalLeftClosed(boolean) {#setIsIntervalLeftClosed-boolean-}

<b>@deprecated.</b> Please use the 'isIntervalLeftClosed' property instead. Indicates whether the interval is closed on the left side.

```javascript
setIsIntervalLeftClosed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for ParetoLine chart.

### getMapChartRegionType() {#getMapChartRegionType--}

<b>@deprecated.</b> Please use the 'mapChartRegionType' property instead. Gets and sets the region type of the map.

```javascript
getMapChartRegionType() : MapChartRegionType;
```


**Returns**

[MapChartRegionType](../mapchartregiontype/)

**Remarks**

Only for map chart.

### setMapChartRegionType(MapChartRegionType) {#setMapChartRegionType-mapchartregiontype-}

<b>@deprecated.</b> Please use the 'mapChartRegionType' property instead. Gets and sets the region type of the map.

```javascript
setMapChartRegionType(value: MapChartRegionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartRegionType](../mapchartregiontype/) | The value to set. |

**Remarks**

Only for map chart.

### getMapChartProjectionType() {#getMapChartProjectionType--}

<b>@deprecated.</b> Please use the 'mapChartProjectionType' property instead. Gets and sets the projection type of the map.

```javascript
getMapChartProjectionType() : MapChartProjectionType;
```


**Returns**

[MapChartProjectionType](../mapchartprojectiontype/)

**Remarks**

Only for map chart.

### setMapChartProjectionType(MapChartProjectionType) {#setMapChartProjectionType-mapchartprojectiontype-}

<b>@deprecated.</b> Please use the 'mapChartProjectionType' property instead. Gets and sets the projection type of the map.

```javascript
setMapChartProjectionType(value: MapChartProjectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartProjectionType](../mapchartprojectiontype/) | The value to set. |

**Remarks**

Only for map chart.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



