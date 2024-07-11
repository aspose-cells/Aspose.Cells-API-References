---
title: RevisionLogCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all revision logs.
type: docs
url: /nodejs-cpp/revisionlogcollection/
---

## RevisionLogCollection class

Represents all revision logs.

```javascript
class RevisionLogCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [RevisionLog](./revisionlog/) by index. |
| [getDaysPreservingHistory()](#getDaysPreservingHistory--)| Gets and sets the number of days the spreadsheet application will keep the change history for this workbook. |
| [setDaysPreservingHistory(number)](#setDaysPreservingHistory-number-)| Gets and sets the number of days the spreadsheet application will keep the change history for this workbook. |
| [highlightChanges(HighlightChangesOptions)](#highlightChanges-highlightchangesoptions-)| Highlights changes of shared workbook. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets [RevisionLog](./revisionlog/) by index.

```javascript
get(index: number) : RevisionLog;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

Returns [RevisionLog](./revisionlog/) object.

### getDaysPreservingHistory() {#getDaysPreservingHistory--}

Gets and sets the number of days the spreadsheet application will keep the change history for this workbook.

```javascript
getDaysPreservingHistory() : number;
```


### setDaysPreservingHistory(number) {#setDaysPreservingHistory-number-}

Gets and sets the number of days the spreadsheet application will keep the change history for this workbook.

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
| options | [HighlightChangesOptions](./highlightchangesoptions/) | Set the options for filtering which changes should be tracked. |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



