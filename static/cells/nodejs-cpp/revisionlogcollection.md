##RevisionLogCollection
Represents all revision logs.
## RevisionLogCollection class
Represents all revision logs.
```javascript
class RevisionLogCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [daysPreservingHistory](#daysPreservingHistory--)| number | Gets and sets the number of days the spreadsheet application will keep the change history for this workbook. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [RevisionLog](../revisionlog/) by index. |
| [getDaysPreservingHistory()](#getDaysPreservingHistory--)| <b>@deprecated.</b> Please use the 'daysPreservingHistory' property instead. Gets and sets the number of days the spreadsheet application will keep the change history for this workbook. |
| [setDaysPreservingHistory(number)](#setDaysPreservingHistory-number-)| <b>@deprecated.</b> Please use the 'daysPreservingHistory' property instead. Gets and sets the number of days the spreadsheet application will keep the change history for this workbook. |
| [highlightChanges(HighlightChangesOptions)](#highlightChanges-highlightchangesoptions-)| Highlights changes of shared workbook. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### daysPreservingHistory {#daysPreservingHistory--}
Gets and sets the number of days the spreadsheet application will keep the change history for this workbook.
```javascript
daysPreservingHistory : number;
```
### get(number) {#get-number-}
Gets [RevisionLog](../revisionlog/) by index.
```javascript
get(index: number) : RevisionLog;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
Returns [RevisionLog](../revisionlog/) object.
### getDaysPreservingHistory() {#getDaysPreservingHistory--}
```javascript
getDaysPreservingHistory() : number;
```
### setDaysPreservingHistory(number) {#setDaysPreservingHistory-number-}
```javascript
setDaysPreservingHistory(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### highlightChanges(HighlightChangesOptions) {#highlightChanges-highlightchangesoptions-}
Highlights changes of shared workbook.
```javascript
highlightChanges(options: HighlightChangesOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [HighlightChangesOptions](../highlightchangesoptions/) | Set the options for filtering which changes should be tracked. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
