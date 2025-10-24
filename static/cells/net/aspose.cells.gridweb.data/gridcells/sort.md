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
GridWeb GridWeb1 = new GridWeb();
GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);
[VB]
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)
```
### See Also
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}
Sorts the datas ascend/decend top to bottom in a range of a Worksheet by specified column index. Sorts the datas ascend/decend left to right in a range of a Worksheet by specified row index.
```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes,
SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to sort. |
| startColumn | Int32 | The column number of the first cell to sort. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| indexes | Int32[] | The column index array that specifis the sort column. if the Orientation is top to bottom ,it stand for the column index that specifis the sort column. if the Orientation is from left to right,it stand for the row index that specifis the sort row. |
| orders | SortByOrder[] | the the sorting order array . |
| orientation | SortOrientation | sorting orientation |
| isCaseSensitive | Boolean | whether the sort is casesensitive . |
### Examples
```csharp
[C#]
GridWeb GridWeb1=new GridWeb();
int[] ids={0,1};
SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);
[VB]
GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)
```
### See Also
* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
