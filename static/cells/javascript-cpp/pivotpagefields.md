##PivotPageFields
Represents the pivot page field items if the pivot table data source is consolidation ranges. It only can contain up to 4 fields.
## PivotPageFields class
Represents the pivot page field items if the pivot table data source is consolidation ranges. It only can contain up to 4 fields.
```javascript
class PivotPageFields;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Represents the pivot page field items. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pageFieldCount](#pageFieldCount--)| number | Readonly. Gets the number of page fields. |
## Methods
| Method | Description |
| --- | --- |
| [addPageField(string[])](#addPageField-stringarray-)| Adds a page field. |
| [addIdentify(number, number[])](#addIdentify-number-numberarray-)| Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first. |
### constructor() {#constructor--}
Represents the pivot page field items.
```javascript
constructor();
```
### pageFieldCount {#pageFieldCount--}
Readonly. Gets the number of page fields.
```javascript
pageFieldCount : number;
```
### addPageField(string[]) {#addPageField-stringarray-}
Adds a page field.
```javascript
addPageField(pageItems: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageItems | string[] | Page field item label |
### addIdentify(number, number[]) {#addIdentify-number-numberarray-}
Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.
```javascript
addIdentify(rangeIndex: number, pageItemIndex: number[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | number | The consolidation data range index. |
| pageItemIndex | number[] | The page item index in the each page field. 		/// pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. 		/// pageItemIndex[1] = -1 means no item in the second field to use to identify this range  		/// and MS will auto create "blank" item in the second field  to identify this range. 		 |
