##LoadFilter
Represents the filter that provides options for loading data when loading workbook from template.
## LoadFilter class
Represents the filter that provides options for loading data when loading workbook from template.
```javascript
class LoadFilter;
```
### Remarks
User may specify the filter options or implement their own LoadFilter to specify how to load data.
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
| [constructor(LoadDataFilterOptions)](#constructor-loaddatafilteroptions-)| Constructs one LoadFilter with given filter options. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [loadDataFilterOptions](#loadDataFilterOptions--)| LoadDataFilterOptions | The filter options to denote what data should be loaded. |
## Methods
| Method | Description |
| --- | --- |
| abstract [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--)| Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded. |
| abstract [startSheet(Worksheet)](#startSheet-worksheet-)| Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### constructor(LoadDataFilterOptions) {#constructor-loaddatafilteroptions-}
Constructs one LoadFilter with given filter options.
```javascript
constructor(opts: LoadDataFilterOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [LoadDataFilterOptions](../loaddatafilteroptions/) | The default filter options. |
### loadDataFilterOptions {#loadDataFilterOptions--}
The filter options to denote what data should be loaded.
```javascript
loadDataFilterOptions : LoadDataFilterOptions;
```
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded.
```javascript
abstract getSheetsInLoadingOrder() : number[];
```
**Returns**
number[]
### startSheet(Worksheet) {#startSheet-worksheet-}
Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet.
```javascript
abstract startSheet(sheet: Worksheet) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../worksheet/) | The worksheet to be loaded.         /// There are only few properties can be used for the given worksheet object here         /// because most data and properties have not been loaded. The available properties are:         /// Name, Index, VisibilityType |
