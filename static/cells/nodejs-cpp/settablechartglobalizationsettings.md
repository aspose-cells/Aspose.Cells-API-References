##SettableChartGlobalizationSettings
Implementation of PivotGlobalizationSettings that supports user to setchange predefined texts.
## SettableChartGlobalizationSettings class
Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.
```javascript
class SettableChartGlobalizationSettings;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [setSeriesName(string)](#setSeriesName-string-)| Sets the name of Series in the Chart. |
| [setChartTitleName(string)](#setChartTitleName-string-)| Sets the name of Chart Title. |
| [setLegendIncreaseName(string)](#setLegendIncreaseName-string-)| Sets the name of increase for Legend. |
| [setLegendDecreaseName(string)](#setLegendDecreaseName-string-)| Sets the name of Decrease for Legend. |
| [setLegendTotalName(string)](#setLegendTotalName-string-)| Sets the name of Total for Legend. |
| [setAxisTitleName(string)](#setAxisTitleName-string-)| Sets the name of Title for Axis. |
| [setOtherName(string)](#setOtherName-string-)| Sets the name of "Other" labels for Chart. |
| [setAxisUnitName(DisplayUnitType, string)](#setAxisUnitName-displayunittype-string-)| Sets the Name of Axis Unit. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSeriesName()](#getSeriesName--)| Gets the name of Series in the Chart. |
| [getChartTitleName()](#getChartTitleName--)| Gets the name of Chart Title. |
| [getLegendIncreaseName()](#getLegendIncreaseName--)| Gets the name of increase for Legend. |
| [getLegendDecreaseName()](#getLegendDecreaseName--)| Gets the name of Decrease for Legend. |
| [getLegendTotalName()](#getLegendTotalName--)| Gets the name of Total for Legend. |
| [getAxisTitleName()](#getAxisTitleName--)| Gets the name of Title for Axis. |
| [getOtherName()](#getOtherName--)| Gets the name of "Other" labels for Chart. |
| [getAxisUnitName(DisplayUnitType)](#getAxisUnitName-displayunittype-)| Gets the Name of Axis Unit. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### setSeriesName(string) {#setSeriesName-string-}
Sets the name of Series in the Chart.
```javascript
setSeriesName(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | local dependent name |
### setChartTitleName(string) {#setChartTitleName-string-}
Sets the name of Chart Title.
```javascript
setChartTitleName(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | local dependent name |
### setLegendIncreaseName(string) {#setLegendIncreaseName-string-}
Sets the name of increase for Legend.
```javascript
setLegendIncreaseName(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | local dependent name |
### setLegendDecreaseName(string) {#setLegendDecreaseName-string-}
Sets the name of Decrease for Legend.
```javascript
setLegendDecreaseName(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | local dependent name |
### setLegendTotalName(string) {#setLegendTotalName-string-}
Sets the name of Total for Legend.
```javascript
setLegendTotalName(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | local dependent name |
### setAxisTitleName(string) {#setAxisTitleName-string-}
Sets the name of Title for Axis.
```javascript
setAxisTitleName(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | local dependent name |
### setOtherName(string) {#setOtherName-string-}
Sets the name of "Other" labels for Chart.
```javascript
setOtherName(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | local dependent name |
### setAxisUnitName(DisplayUnitType, string) {#setAxisUnitName-displayunittype-string-}
Sets the Name of Axis Unit.
```javascript
setAxisUnitName(type: DisplayUnitType, name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DisplayUnitType](../displayunittype/) | The unit type for displaying axis labels. |
| name | string | local dependent name |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getSeriesName() {#getSeriesName--}
Gets the name of Series in the Chart.
```javascript
getSeriesName() : string;
```
### getChartTitleName() {#getChartTitleName--}
Gets the name of Chart Title.
```javascript
getChartTitleName() : string;
```
### getLegendIncreaseName() {#getLegendIncreaseName--}
Gets the name of increase for Legend.
```javascript
getLegendIncreaseName() : string;
```
### getLegendDecreaseName() {#getLegendDecreaseName--}
Gets the name of Decrease for Legend.
```javascript
getLegendDecreaseName() : string;
```
### getLegendTotalName() {#getLegendTotalName--}
Gets the name of Total for Legend.
```javascript
getLegendTotalName() : string;
```
### getAxisTitleName() {#getAxisTitleName--}
Gets the name of Title for Axis.
```javascript
getAxisTitleName() : string;
```
### getOtherName() {#getOtherName--}
Gets the name of "Other" labels for Chart.
```javascript
getOtherName() : string;
```
### getAxisUnitName(DisplayUnitType) {#getAxisUnitName-displayunittype-}
Gets the Name of Axis Unit.
```javascript
getAxisUnitName(type: DisplayUnitType) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [DisplayUnitType](../displayunittype/) |  |
