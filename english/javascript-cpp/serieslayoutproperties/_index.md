---
title: SeriesLayoutProperties
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the properties of series layout.
type: docs
url: /javascript-cpp/serieslayoutproperties/
---

## SeriesLayoutProperties class

Represents the properties of series layout.

```javascript
class SeriesLayoutProperties;
```

### Remarks
Only applicable to BoxWhisker,Funnel,ParetoLine,Sunburst,Treemap,Waterfall and Histogram chart.

## Constructors

| Name | Description |
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


