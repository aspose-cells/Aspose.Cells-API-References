##PivotFormatConditionCollection
Represents PivotTable Format Conditions.
## PivotFormatConditionCollection class
Represents PivotTable Format Conditions.
```javascript
class PivotFormatConditionCollection;
```
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotConditionalFormatCollection class. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of conditional formats. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the pivot FormatCondition object at the specific index. |
| [add()](#add--)| Adds a pivot FormatCondition to the collection. |
| [removeAt(number)](#removeAt-number-)| Remove a conditional formats. |
### count {#count--}
Readonly. Gets the count of conditional formats.
```javascript
count : number;
```
### get(number) {#get-number-}
Gets the pivot FormatCondition object at the specific index.
```javascript
get(index: number) : PivotFormatCondition;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
pivot FormatCondition object.
### add() {#add--}
Adds a pivot FormatCondition to the collection.
```javascript
add() : number;
```
**Returns**
pivot FormatCondition object index.
**Remarks**
not supported
### removeAt(number) {#removeAt-number-}
Remove a conditional formats.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
