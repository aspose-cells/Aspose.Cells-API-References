##PivotTableCalculateOption
Rerepsents the options of calcuating the pivot table.
## PivotTableCalculateOption class
Rerepsents the options of calcuating the pivot table.
```javascript
class PivotTableCalculateOption;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [refreshData](#refreshData--)| boolean | Indicates whether refreshing data source of the pivottable. |
| [refreshCharts](#refreshCharts--)| boolean | Indicates whether refreshing charts are based on this pivot table. |
| [reserveMissingPivotItemType](#reserveMissingPivotItemType--)| ReserveMissingPivotItemType | Represents how to reserve missing pivot items. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### refreshData {#refreshData--}
Indicates whether refreshing data source of the pivottable.
```javascript
refreshData : boolean;
```
### refreshCharts {#refreshCharts--}
Indicates whether refreshing charts are based on this pivot table.
```javascript
refreshCharts : boolean;
```
### reserveMissingPivotItemType {#reserveMissingPivotItemType--}
Represents how to reserve missing pivot items.
```javascript
reserveMissingPivotItemType : ReserveMissingPivotItemType;
```
**Remarks**
Only works when [RefreshData](../refreshdata/) is true.
