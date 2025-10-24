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
| [highlightChanges(HighlightChangesOptions)](#highlightChanges-highlightchangesoptions-)| Highlights changes of shared workbook. |
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
### highlightChanges(HighlightChangesOptions) {#highlightChanges-highlightchangesoptions-}
Highlights changes of shared workbook.
```javascript
highlightChanges(options: HighlightChangesOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [HighlightChangesOptions](../highlightchangesoptions/) | Set the options for filtering which changes should be tracked. |
