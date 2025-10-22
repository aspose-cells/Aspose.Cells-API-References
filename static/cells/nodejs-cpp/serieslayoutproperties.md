##SeriesLayoutProperties
Represents the properties of series layout.
## SeriesLayoutProperties class
Represents the properties of series layout.
```javascript
class SeriesLayoutProperties;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [showConnectorLines](#showConnectorLines--)| boolean | Indicates whether showing connector lines between data points. |
| [showMeanLine](#showMeanLine--)| boolean | Indicates whether showing the line connecting all mean points. |
| [showOutlierPoints](#showOutlierPoints--)| boolean | Indicates whether showing outlier data points. |
| [showMeanMarker](#showMeanMarker--)| boolean | Indicates whether showing markers denoting the mean. |
| [showInnerPoints](#showInnerPoints--)| boolean | Indicates whether showing non-outlier data points. |
| [subtotals](#subtotals--)| number[] | Represents the index of a subtotal data point. |
| [quartileCalculation](#quartileCalculation--)| QuartileCalculationType | Represents the statistical properties for the series. |
| [mapLabelLayout](#mapLabelLayout--)| MapChartLabelLayout | Gets and sets the layout of map labels. |
| [isIntervalLeftClosed](#isIntervalLeftClosed--)| boolean | Indicates whether the interval is closed on the left side. |
| [mapChartRegionType](#mapChartRegionType--)| MapChartRegionType | Gets and sets the region type of the map. |
| [mapChartProjectionType](#mapChartProjectionType--)| MapChartProjectionType | Gets and sets the projection type of the map. |
## Methods
| Method | Description |
| --- | --- |
| [getShowConnectorLines()](#getShowConnectorLines--)| <b>@deprecated.</b> Please use the 'showConnectorLines' property instead. Indicates whether showing connector lines between data points. |
| [setShowConnectorLines(boolean)](#setShowConnectorLines-boolean-)| <b>@deprecated.</b> Please use the 'showConnectorLines' property instead. Indicates whether showing connector lines between data points. |
| [getShowMeanLine()](#getShowMeanLine--)| <b>@deprecated.</b> Please use the 'showMeanLine' property instead. Indicates whether showing the line connecting all mean points. |
| [setShowMeanLine(boolean)](#setShowMeanLine-boolean-)| <b>@deprecated.</b> Please use the 'showMeanLine' property instead. Indicates whether showing the line connecting all mean points. |
| [getShowOutlierPoints()](#getShowOutlierPoints--)| <b>@deprecated.</b> Please use the 'showOutlierPoints' property instead. Indicates whether showing outlier data points. |
| [setShowOutlierPoints(boolean)](#setShowOutlierPoints-boolean-)| <b>@deprecated.</b> Please use the 'showOutlierPoints' property instead. Indicates whether showing outlier data points. |
| [getShowMeanMarker()](#getShowMeanMarker--)| <b>@deprecated.</b> Please use the 'showMeanMarker' property instead. Indicates whether showing markers denoting the mean. |
| [setShowMeanMarker(boolean)](#setShowMeanMarker-boolean-)| <b>@deprecated.</b> Please use the 'showMeanMarker' property instead. Indicates whether showing markers denoting the mean. |
| [getShowInnerPoints()](#getShowInnerPoints--)| <b>@deprecated.</b> Please use the 'showInnerPoints' property instead. Indicates whether showing non-outlier data points. |
| [setShowInnerPoints(boolean)](#setShowInnerPoints-boolean-)| <b>@deprecated.</b> Please use the 'showInnerPoints' property instead. Indicates whether showing non-outlier data points. |
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
Indicates whether showing connector lines between data points.
```javascript
showConnectorLines : boolean;
```
### showMeanLine {#showMeanLine--}
Indicates whether showing the line connecting all mean points.
```javascript
showMeanLine : boolean;
```
### showOutlierPoints {#showOutlierPoints--}
Indicates whether showing outlier data points.
```javascript
showOutlierPoints : boolean;
```
### showMeanMarker {#showMeanMarker--}
Indicates whether showing markers denoting the mean.
```javascript
showMeanMarker : boolean;
```
### showInnerPoints {#showInnerPoints--}
Indicates whether showing non-outlier data points.
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
### mapChartRegionType {#mapChartRegionType--}
Gets and sets the region type of the map.
```javascript
mapChartRegionType : MapChartRegionType;
```
### mapChartProjectionType {#mapChartProjectionType--}
Gets and sets the projection type of the map.
```javascript
mapChartProjectionType : MapChartProjectionType;
```
### getShowConnectorLines() {#getShowConnectorLines--}
```javascript
getShowConnectorLines() : boolean;
```
### setShowConnectorLines(boolean) {#setShowConnectorLines-boolean-}
```javascript
setShowConnectorLines(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowMeanLine() {#getShowMeanLine--}
```javascript
getShowMeanLine() : boolean;
```
### setShowMeanLine(boolean) {#setShowMeanLine-boolean-}
```javascript
setShowMeanLine(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowOutlierPoints() {#getShowOutlierPoints--}
```javascript
getShowOutlierPoints() : boolean;
```
### setShowOutlierPoints(boolean) {#setShowOutlierPoints-boolean-}
```javascript
setShowOutlierPoints(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowMeanMarker() {#getShowMeanMarker--}
```javascript
getShowMeanMarker() : boolean;
```
### setShowMeanMarker(boolean) {#setShowMeanMarker-boolean-}
```javascript
setShowMeanMarker(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getShowInnerPoints() {#getShowInnerPoints--}
```javascript
getShowInnerPoints() : boolean;
```
### setShowInnerPoints(boolean) {#setShowInnerPoints-boolean-}
```javascript
setShowInnerPoints(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSubtotals() {#getSubtotals--}
```javascript
getSubtotals() : number[];
```
**Returns**
number[]
### setSubtotals(number[]) {#setSubtotals-numberarray-}
```javascript
setSubtotals(value: number[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### getQuartileCalculation() {#getQuartileCalculation--}
```javascript
getQuartileCalculation() : QuartileCalculationType;
```
**Returns**
[QuartileCalculationType](../quartilecalculationtype/)
### setQuartileCalculation(QuartileCalculationType) {#setQuartileCalculation-quartilecalculationtype-}
```javascript
setQuartileCalculation(value: QuartileCalculationType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [QuartileCalculationType](../quartilecalculationtype/) | The value to set. |
### getMapLabelLayout() {#getMapLabelLayout--}
```javascript
getMapLabelLayout() : MapChartLabelLayout;
```
**Returns**
[MapChartLabelLayout](../mapchartlabellayout/)
### setMapLabelLayout(MapChartLabelLayout) {#setMapLabelLayout-mapchartlabellayout-}
```javascript
setMapLabelLayout(value: MapChartLabelLayout) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartLabelLayout](../mapchartlabellayout/) | The value to set. |
### isIntervalLeftClosed() {#isIntervalLeftClosed--}
```javascript
isIntervalLeftClosed() : boolean;
```
### setIsIntervalLeftClosed(boolean) {#setIsIntervalLeftClosed-boolean-}
```javascript
setIsIntervalLeftClosed(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getMapChartRegionType() {#getMapChartRegionType--}
```javascript
getMapChartRegionType() : MapChartRegionType;
```
**Returns**
[MapChartRegionType](../mapchartregiontype/)
### setMapChartRegionType(MapChartRegionType) {#setMapChartRegionType-mapchartregiontype-}
```javascript
setMapChartRegionType(value: MapChartRegionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartRegionType](../mapchartregiontype/) | The value to set. |
### getMapChartProjectionType() {#getMapChartProjectionType--}
```javascript
getMapChartProjectionType() : MapChartProjectionType;
```
**Returns**
[MapChartProjectionType](../mapchartprojectiontype/)
### setMapChartProjectionType(MapChartProjectionType) {#setMapChartProjectionType-mapchartprojectiontype-}
```javascript
setMapChartProjectionType(value: MapChartProjectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MapChartProjectionType](../mapchartprojectiontype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
