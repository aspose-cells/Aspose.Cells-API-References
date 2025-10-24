##GridCells.Sort
GridCells method. Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}
Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index.
```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending,
bool isCaseSensitive, bool islefttoright)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to sort. |
| startColumn | Int32 | The column number of the first cell to sort. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| index | Int32 | The column index that specifis the sort column. if the Orientation is top to bottom ,it stand for the column index that specifis the sort column. if the Orientation is from left to right,it stand for the row index that specifis the sort row. |
| isAsending | Boolean | whether the sorting order is asending . |
| isCaseSensitive | Boolean | whether the sort is casesensitive . |
| islefttoright | Boolean | whether the sort orientation is from left to right |
### Examples
```csharp
[C#]
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);
[VB]
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)
```
### See Also
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}
Sorts the data of the area.
```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes,
SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```
| Parameter | Description |
| --- | --- |
| cells | The cells contains the data area. |
| startRow | The start row of the area. |
| startColumn | The start column of the area. |
| rows | the total rows. |
| columns | The total columns. |
| indexes | The sorted column index array |
| orders | The sorted order array |
| orientation | the sorting orientation:from left to right or from top to bottom. |
| isCaseSensitive | whether case sensitive when comparing string.. |
### See Also
* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
