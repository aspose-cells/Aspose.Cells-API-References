##ChartGlobalizationSettings
Represents the globalization settings for chart.
## ChartGlobalizationSettings class
Represents the globalization settings for chart.
```javascript
class ChartGlobalizationSettings;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| abstract [getSeriesName()](#getSeriesName--)| Gets the name of Series in the Chart. |
| abstract [getChartTitleName()](#getChartTitleName--)| Gets the name of Chart Title. |
| abstract [getLegendIncreaseName()](#getLegendIncreaseName--)| Gets the name of increase for Legend. |
| abstract [getLegendDecreaseName()](#getLegendDecreaseName--)| Gets the name of Decrease for Legend. |
| abstract [getLegendTotalName()](#getLegendTotalName--)| Gets the name of Total for Legend. |
| abstract [getAxisTitleName()](#getAxisTitleName--)| Gets the name of Title for Axis. |
| abstract [getOtherName()](#getOtherName--)| Gets the name of "Other" labels for Chart. |
| abstract [getAxisUnitName(DisplayUnitType)](#getAxisUnitName-displayunittype-)| Gets the Name of Axis Unit. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### getSeriesName() {#getSeriesName--}
Gets the name of Series in the Chart.
```javascript
abstract getSeriesName() : string;
```
### getChartTitleName() {#getChartTitleName--}
Gets the name of Chart Title.
```javascript
abstract getChartTitleName() : string;
```
### getLegendIncreaseName() {#getLegendIncreaseName--}
Gets the name of increase for Legend.
```javascript
abstract getLegendIncreaseName() : string;
```
### getLegendDecreaseName() {#getLegendDecreaseName--}
Gets the name of Decrease for Legend.
```javascript
abstract getLegendDecreaseName() : string;
```
### getLegendTotalName() {#getLegendTotalName--}
Gets the name of Total for Legend.
```javascript
abstract getLegendTotalName() : string;
```
### getAxisTitleName() {#getAxisTitleName--}
Gets the name of Title for Axis.
```javascript
abstract getAxisTitleName() : string;
```
### getOtherName() {#getOtherName--}
Gets the name of "Other" labels for Chart.
```javascript
abstract getOtherName() : string;
```
### getAxisUnitName(DisplayUnitType) {#getAxisUnitName-displayunittype-}
Gets the Name of Axis Unit.
```javascript
abstract getAxisUnitName(type: DisplayUnitType) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DisplayUnitType](../displayunittype/) |  |
