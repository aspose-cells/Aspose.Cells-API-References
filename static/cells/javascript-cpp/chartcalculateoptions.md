##ChartCalculateOptions
Represents the options for calculating chart.
## ChartCalculateOptions class
Represents the options for calculating chart.
```javascript
class ChartCalculateOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for calculating chart. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [updateAllPoints](#updateAllPoints--)| boolean | Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger. |
### constructor() {#constructor--}
Creates the options for calculating chart.
```javascript
constructor();
```
### updateAllPoints {#updateAllPoints--}
Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.
```javascript
updateAllPoints : boolean;
```
