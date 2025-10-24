##TimelineCollection
Specifies the collection of all the Timeline objects on the specified worksheet. Due to MS Excel Excel 2003 does not support Timeline.
## TimelineCollection class
Specifies the collection of all the Timeline objects on the specified worksheet. Due to MS Excel, Excel 2003 does not support Timeline.
```javascript
class TimelineCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the Timeline by index. |
| [get(string)](#get-string-)| Gets the Timeline  by Timeline's name. |
| [add(PivotTable, number, number, string)](#add-pivottable-number-number-string-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, string, string)](#add-pivottable-string-string-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, number, number, number)](#add-pivottable-number-number-number-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, string, number)](#add-pivottable-string-number-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, number, number, PivotField)](#add-pivottable-number-number-pivotfield-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, string, PivotField)](#add-pivottable-string-pivotfield-)| Add a new Timeline using PivotTable as data source |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the Timeline by index.
```javascript
get(index: number) : Timeline;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
[Timeline](../timeline/)
### get(string) {#get-string-}
Gets the Timeline  by Timeline's name.
```javascript
get(name: string) : Timeline;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |
**Returns**
[Timeline](../timeline/)
### add(PivotTable, number, number, string) {#add-pivottable-number-number-string-}
Add a new Timeline using PivotTable as data source
```javascript
add(pivot: PivotTable, row: number, column: number, baseFieldName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldName | string | The name of PivotField in PivotTable.BaseFields |
**Returns**
The new add Timeline index
### add(PivotTable, string, string) {#add-pivottable-string-string-}
Add a new Timeline using PivotTable as data source
```javascript
add(pivot: PivotTable, destCellName: string, baseFieldName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| destCellName | string | The cell name in the upper-left corner of the Timeline range. |
| baseFieldName | string | The name of PivotField in PivotTable.BaseFields |
**Returns**
The new add Timeline index
### add(PivotTable, number, number, number) {#add-pivottable-number-number-number-}
Add a new Timeline using PivotTable as data source
```javascript
add(pivot: PivotTable, row: number, column: number, baseFieldIndex: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldIndex | number | The index of PivotField in PivotTable.BaseFields |
**Returns**
The new add Timeline index
### add(PivotTable, string, number) {#add-pivottable-string-number-}
Add a new Timeline using PivotTable as data source
```javascript
add(pivot: PivotTable, destCellName: string, baseFieldIndex: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| destCellName | string | The cell name in the upper-left corner of the Timeline range. |
| baseFieldIndex | number | The index of PivotField in PivotTable.BaseFields |
**Returns**
The new add Timeline index
### add(PivotTable, number, number, PivotField) {#add-pivottable-number-number-pivotfield-}
Add a new Timeline using PivotTable as data source
```javascript
add(pivot: PivotTable, row: number, column: number, baseField: PivotField) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseField | [PivotField](../pivotfield/) | The PivotField in PivotTable.BaseFields |
**Returns**
The new add Timeline index
### add(PivotTable, string, PivotField) {#add-pivottable-string-pivotfield-}
Add a new Timeline using PivotTable as data source
```javascript
add(pivot: PivotTable, destCellName: string, baseField: PivotField) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| destCellName | string | The cell name in the upper-left corner of the Timeline range. |
| baseField | [PivotField](../pivotfield/) | The PivotField in PivotTable.BaseFields |
**Returns**
The new add Timeline index
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
