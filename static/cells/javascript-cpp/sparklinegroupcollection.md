##SparklineGroupCollection
Encapsulates a collection of SparklineGroup..sparklinegroup objects.
## SparklineGroupCollection class
Encapsulates a collection of [SparklineGroup](../sparklinegroup/) objects.
```javascript
class SparklineGroupCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [SparklineGroup](../sparklinegroup/) element at the specified index. |
| [add(SparklineType)](#add-sparklinetype-)| Adds an [SparklineGroup](../sparklinegroup/) with a [Sparkline](../sparkline/) to the collection. |
| [add(SparklineType, string, boolean, CellArea)](#add-sparklinetype-string-boolean-cellarea-)| Adds an [SparklineGroup](../sparklinegroup/) with [Sparkline](../sparkline/) to the collection. |
| [clearSparklines(CellArea)](#clearSparklines-cellarea-)| Clears the sparklines that is inside an area of cells. |
| [clearSparklineGroups(CellArea)](#clearSparklineGroups-cellarea-)| Clears the sparkline groups that overlaps an area of cells. |
### get(number) {#get-number-}
Gets the [SparklineGroup](../sparklinegroup/) element at the specified index.
```javascript
get(index: number) : SparklineGroup;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(SparklineType) {#add-sparklinetype-}
Adds an [SparklineGroup](../sparklinegroup/) with a [Sparkline](../sparkline/) to the collection.
```javascript
add(type: SparklineType) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [SparklineType](../sparklinetype/) | Specifies the type of the Sparkline group. |
**Returns**
[SparklineGroup](../sparklinegroup/) object index.
### add(SparklineType, string, boolean, CellArea) {#add-sparklinetype-string-boolean-cellarea-}
Adds an [SparklineGroup](../sparklinegroup/) with [Sparkline](../sparkline/) to the collection.
```javascript
add(type: SparklineType, dataRange: string, isVertical: boolean, locationRange: CellArea) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [SparklineType](../sparklinetype/) | Specifies the type of the Sparkline group. |
| dataRange | string | Specifies the data range of the sparkline group. |
| isVertical | boolean | Specifies whether to plot the sparklines from the data range by row or by column. |
| locationRange | [CellArea](../cellarea/) | Specifies where the sparklines to be placed. |
**Returns**
[SparklineGroup](../sparklinegroup/) object index.
### clearSparklines(CellArea) {#clearSparklines-cellarea-}
Clears the sparklines that is inside an area of cells.
```javascript
clearSparklines(cellArea: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Specifies the area of cells |
### clearSparklineGroups(CellArea) {#clearSparklineGroups-cellarea-}
Clears the sparkline groups that overlaps an area of cells.
```javascript
clearSparklineGroups(cellArea: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Specifies the area of cells |
