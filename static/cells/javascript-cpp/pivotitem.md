##PivotItem
Represents a item in a PivotField report.
## PivotItem class
Represents a item in a PivotField report.
```javascript
class PivotItem;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isHidden](#isHidden--)| boolean | Gets and Sets whether the pivot item is hidden. |
| [position](#position--)| number | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [positionInSameParentNode](#positionInSameParentNode--)| number | Specifying the position index in the PivotItems under the same parent node. |
| [isDetailHidden](#isDetailHidden--)| boolean | Gets and sets whether the detail of this pivot item is hidden. |
| [isCalculatedItem](#isCalculatedItem--)| boolean | Readonly. Indicates whether this pivot item is a calculated formula item. |
| [isMissing](#isMissing--)| boolean | Readonly. Indicates whether the item is removed from the data source. |
| [value](#value--)| VObject | Readonly. Gets the value of the pivot item |
| [name](#name--)| string | Gets the name of the pivot item. |
| [index](#index--)| number | Gets the index of the pivot item in cache field. |
## Methods
| Method | Description |
| --- | --- |
| [move(number, boolean)](#move-number-boolean-)| Moves the item up or down |
| [getFormula()](#getFormula--)| Gets the formula of this calculated item. Only works when this item is calculated item. |
| [getStringValue()](#getStringValue--)| Gets the string value of the pivot item If the value is null, it will return "" |
| [getDoubleValue()](#getDoubleValue--)| Gets the double value of the pivot item If the value is null or not number ,it will return 0 |
| [getDateTimeValue()](#getDateTimeValue--)| Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue |
### isHidden {#isHidden--}
Gets and Sets whether the pivot item is hidden.
```javascript
isHidden : boolean;
```
### position {#position--}
Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.
```javascript
position : number;
```
### positionInSameParentNode {#positionInSameParentNode--}
Specifying the position index in the PivotItems under the same parent node.
```javascript
positionInSameParentNode : number;
```
### isDetailHidden {#isDetailHidden--}
Gets and sets whether the detail of this pivot item is hidden.
```javascript
isDetailHidden : boolean;
```
### isCalculatedItem {#isCalculatedItem--}
Readonly. Indicates whether this pivot item is a calculated formula item.
```javascript
isCalculatedItem : boolean;
```
### isMissing {#isMissing--}
Readonly. Indicates whether the item is removed from the data source.
```javascript
isMissing : boolean;
```
**Remarks**
True means this value has benn removed from the data source.
### value {#value--}
Readonly. Gets the value of the pivot item
```javascript
value : VObject;
```
### name {#name--}
Gets the name of the pivot item.
```javascript
name : string;
```
### index {#index--}
Gets the index of the pivot item in cache field.
```javascript
index : number;
```
### move(number, boolean) {#move-number-boolean-}
Moves the item up or down
```javascript
move(count: number, isSameParent: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| count | number | The number of moving up or down.         /// Move the item up if this is less than zero;         /// Move the item down if this is greater than zero. |
| isSameParent | boolean | Specifying whether moving operation is in the same parent node or not |
### getFormula() {#getFormula--}
Gets the formula of this calculated item. Only works when this item is calculated item.
```javascript
getFormula() : string;
```
### getStringValue() {#getStringValue--}
Gets the string value of the pivot item If the value is null, it will return ""
```javascript
getStringValue() : string;
```
### getDoubleValue() {#getDoubleValue--}
Gets the double value of the pivot item If the value is null or not number ,it will return 0
```javascript
getDoubleValue() : number;
```
### getDateTimeValue() {#getDateTimeValue--}
Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue
```javascript
getDateTimeValue() : Date;
```
