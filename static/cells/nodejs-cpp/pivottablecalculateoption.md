##PivotTableCalculateOption
Rerepsents the options of calcuating the pivot table.
## PivotTableCalculateOption class
Rerepsents the options of calcuating the pivot table.
```javascript
class PivotTableCalculateOption;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [refreshData](#refreshData--)| boolean | Indicates whether refreshing data source of the pivottable. |
| [refreshCharts](#refreshCharts--)| boolean | Indicates whether refreshing charts are based on this pivot table. |
| [reserveMissingPivotItemType](#reserveMissingPivotItemType--)| ReserveMissingPivotItemType | Represents how to reserve missing pivot items. |
## Methods
| Method | Description |
| --- | --- |
| [getRefreshData()](#getRefreshData--)| <b>@deprecated.</b> Please use the 'refreshData' property instead. Indicates whether refreshing data source of the pivottable. |
| [setRefreshData(boolean)](#setRefreshData-boolean-)| <b>@deprecated.</b> Please use the 'refreshData' property instead. Indicates whether refreshing data source of the pivottable. |
| [getRefreshCharts()](#getRefreshCharts--)| <b>@deprecated.</b> Please use the 'refreshCharts' property instead. Indicates whether refreshing charts are based on this pivot table. |
| [setRefreshCharts(boolean)](#setRefreshCharts-boolean-)| <b>@deprecated.</b> Please use the 'refreshCharts' property instead. Indicates whether refreshing charts are based on this pivot table. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--)| <b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items. |
| [setReserveMissingPivotItemType(ReserveMissingPivotItemType)](#setReserveMissingPivotItemType-reservemissingpivotitemtype-)| <b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getRefreshData() {#getRefreshData--}
```javascript
getRefreshData() : boolean;
```
### setRefreshData(boolean) {#setRefreshData-boolean-}
```javascript
setRefreshData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshCharts() {#getRefreshCharts--}
```javascript
getRefreshCharts() : boolean;
```
### setRefreshCharts(boolean) {#setRefreshCharts-boolean-}
```javascript
setRefreshCharts(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```javascript
getReserveMissingPivotItemType() : ReserveMissingPivotItemType;
```
**Returns**
[ReserveMissingPivotItemType](../reservemissingpivotitemtype/)
**Remarks**
Only works when [RefreshData](../refreshdata/) is true.
### setReserveMissingPivotItemType(ReserveMissingPivotItemType) {#setReserveMissingPivotItemType-reservemissingpivotitemtype-}
```javascript
setReserveMissingPivotItemType(value: ReserveMissingPivotItemType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReserveMissingPivotItemType](../reservemissingpivotitemtype/) | The value to set. |
**Remarks**
Only works when [RefreshData](../refreshdata/) is true.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
