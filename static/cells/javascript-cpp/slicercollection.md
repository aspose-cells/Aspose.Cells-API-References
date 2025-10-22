##SlicerCollection
Specifies the collection of all the Slicer objects on the specified worksheet.
## SlicerCollection class
Specifies the collection of all the Slicer objects on the specified worksheet.
```javascript
class SlicerCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the Slicer by index. |
| [get(string)](#get-string-)| Gets the Slicer  by slicer's name. |
| [remove(Slicer)](#remove-slicer-)| Remove the specified Slicer |
| [removeAt(number)](#removeAt-number-)| Deletes the Slicer at the specified index |
| [clear()](#clear--)| Clear all Slicers. |
| [add(PivotTable, string, string)](#add-pivottable-string-string-)| Add a new Slicer using PivotTable as data source |
| [add(PivotTable, number, number, string)](#add-pivottable-number-number-string-)| Add a new Slicer using PivotTable as data source |
| [add(PivotTable, number, number, number)](#add-pivottable-number-number-number-)| Add a new Slicer using PivotTable as data source |
| [add(PivotTable, string, number)](#add-pivottable-string-number-)| Add a new Slicer using PivotTable as data source |
| [add(PivotTable, number, number, PivotField)](#add-pivottable-number-number-pivotfield-)| Add a new Slicer using PivotTable as data source |
| [add(PivotTable, string, PivotField)](#add-pivottable-string-pivotfield-)| Add a new Slicer using PivotTable as data source |
| [add(ListObject, number, string)](#add-listobject-number-string-)| Add a new Slicer using ListObjet as data source |
| [add(ListObject, ListColumn, string)](#add-listobject-listcolumn-string-)| Add a new Slicer using ListObjet as data source |
| [add(ListObject, ListColumn, number, number)](#add-listobject-listcolumn-number-number-)| Add a new Slicer using ListObjet as data source |
### get(number) {#get-number-}
Gets the Slicer by index.
```javascript
get(index: number) : Slicer;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
[Slicer](../slicer/)
### get(string) {#get-string-}
Gets the Slicer  by slicer's name.
```javascript
get(name: string) : Slicer;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |
**Returns**
[Slicer](../slicer/)
### remove(Slicer) {#remove-slicer-}
Remove the specified Slicer
```javascript
remove(slicer: Slicer) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| slicer | [Slicer](../slicer/) | The Slicer object |
### removeAt(number) {#removeAt-number-}
Deletes the Slicer at the specified index
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position index in Slicer collection |
### clear() {#clear--}
Clear all Slicers.
```javascript
clear() : void;
```
### add(PivotTable, string, string) {#add-pivottable-string-string-}
Add a new Slicer using PivotTable as data source
```javascript
add(pivot: PivotTable, destCellName: string, baseFieldName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| destCellName | string | The cell in the upper-left corner of the Slicer range. |
| baseFieldName | string | The name of PivotField in PivotTable.BaseFields |
**Returns**
The new add Slicer index
### add(PivotTable, number, number, string) {#add-pivottable-number-number-string-}
Add a new Slicer using PivotTable as data source
```javascript
add(pivot: PivotTable, row: number, column: number, baseFieldName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | number | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldName | string | The name of PivotField in PivotTable.BaseFields |
**Returns**
The new add Slicer index
### add(PivotTable, number, number, number) {#add-pivottable-number-number-number-}
Add a new Slicer using PivotTable as data source
```javascript
add(pivot: PivotTable, row: number, column: number, baseFieldIndex: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | number | Column index of the cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | number | The index of PivotField in PivotTable.BaseFields |
**Returns**
The new add Slicer index
### add(PivotTable, string, number) {#add-pivottable-string-number-}
Add a new Slicer using PivotTable as data source
```javascript
add(pivot: PivotTable, destCellName: string, baseFieldIndex: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| destCellName | string | The cell in the upper-left corner of the Slicer range. |
| baseFieldIndex | number | The index of PivotField in PivotTable.BaseFields |
**Returns**
The new add Slicer index
### add(PivotTable, number, number, PivotField) {#add-pivottable-number-number-pivotfield-}
Add a new Slicer using PivotTable as data source
```javascript
add(pivot: PivotTable, row: number, column: number, baseField: PivotField) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | number | Column index of the cell in the upper-left corner of the Slicer range. |
| baseField | [PivotField](../pivotfield/) | The PivotField in PivotTable.BaseFields |
**Returns**
The new add Slicer index
### add(PivotTable, string, PivotField) {#add-pivottable-string-pivotfield-}
Add a new Slicer using PivotTable as data source
```javascript
add(pivot: PivotTable, destCellName: string, baseField: PivotField) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](../pivottable/) | PivotTable object |
| destCellName | string | The cell in the upper-left corner of the Slicer range. |
| baseField | [PivotField](../pivotfield/) | The PivotField in PivotTable.BaseFields |
**Returns**
The new add Slicer index
### add(ListObject, number, string) {#add-listobject-number-string-}
Add a new Slicer using ListObjet as data source
```javascript
add(table: ListObject, index: number, destCellName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [ListObject](../listobject/) | ListObject object |
| index | number | The index of ListColumn in ListObject.ListColumns |
| destCellName | string | The cell in the upper-left corner of the Slicer range. |
**Returns**
The new add Slicer index
### add(ListObject, ListColumn, string) {#add-listobject-listcolumn-string-}
Add a new Slicer using ListObjet as data source
```javascript
add(table: ListObject, listColumn: ListColumn, destCellName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [ListObject](../listobject/) | ListObject object |
| listColumn | [ListColumn](../listcolumn/) | The ListColumn in ListObject.ListColumns |
| destCellName | string | The cell in the upper-left corner of the Slicer range. |
**Returns**
The new add Slicer index
### add(ListObject, ListColumn, number, number) {#add-listobject-listcolumn-number-number-}
Add a new Slicer using ListObjet as data source
```javascript
add(table: ListObject, listColumn: ListColumn, row: number, column: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [ListObject](../listobject/) | ListObject object |
| listColumn | [ListColumn](../listcolumn/) | The ListColumn in ListObject.ListColumns |
| row | number | Row index of the cell in the upper-left corner of the Slicer range. |
| column | number | Column index of the cell in the upper-left corner of the Slicer range. |
**Returns**
The new add Slicer index
