##PivotFieldSortSetting
Represents the setting of sorting pivot fields.
## PivotFieldSortSetting class
Represents the setting of sorting pivot fields.
```javascript
class PivotFieldSortSetting;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [sortType](#sortType--)| SortOrder | Readonly. Represents the [SortOrder](../sortorder/). |
| [isSortByLabels](#isSortByLabels--)| boolean | Readonly. Indicates whether sorting the field by itself or data field. |
| [fieldIndex](#fieldIndex--)| number | Readonly. Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field. |
| [lineTypeSortedBy](#lineTypeSortedBy--)| PivotLineType | Readonly. The pivot line type sorted by. |
| [isSimpleSort](#isSimpleSort--)| boolean | Readonly. Indicates whether a simple data sort operation will be applied. |
| [cell](#cell--)| string | Readonly. Sorts by the values in which row or column. |
### sortType {#sortType--}
Readonly. Represents the [SortOrder](../sortorder/).
```javascript
sortType : SortOrder;
```
### isSortByLabels {#isSortByLabels--}
Readonly. Indicates whether sorting the field by itself or data field.
```javascript
isSortByLabels : boolean;
```
### fieldIndex {#fieldIndex--}
Readonly. Represents the index of the field sorted by. -1 means sorting the PivotField by the labels,others means sorting by the data field.
```javascript
fieldIndex : number;
```
### lineTypeSortedBy {#lineTypeSortedBy--}
Readonly. The pivot line type sorted by.
```javascript
lineTypeSortedBy : PivotLineType;
```
**Remarks**
Only works when not sorting this field by labels.
### isSimpleSort {#isSimpleSort--}
Readonly. Indicates whether a simple data sort operation will be applied.
```javascript
isSimpleSort : boolean;
```
**Remarks**
The default value is true.
### cell {#cell--}
Readonly. Sorts by the values in which row or column.
```javascript
cell : string;
```
