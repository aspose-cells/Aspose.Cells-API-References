##WebCells.Sort
WebCells method. Sorts the datas ascend top to bottom in a range of a WebWorksheet by specified column index
## Sort(int, int, int, int, int) {#sort}
Sorts the datas ascend top to bottom in a range of a WebWorksheet by specified column index.
```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to sort. |
| startColumn | Int32 | The column number of the first cell to sort. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| index | Int32 | The column index that specifis the sort column. |
### Examples
```csharp
[C#]
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);
[VB]
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)
```
### See Also
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}
Sorts the datas ascend top to bottom in a range of a WebWorksheet by specified column index.
```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index,
SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to sort. |
| startColumn | Int32 | The column number of the first cell to sort. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| index | Int32 | The column(or row) index that specifis the sort column(or row). If sort orientation is top to bottom, the index represents column index. If sort orientation is left to right, the index represents row index. |
| order | SortByOrder | The sort order:Ascending or Descending |
| orientation | SortOrientation | The sort orientation: top to bottom or left to right. |
| isCaseSensitive | Boolean | Indicates whether the sort data is case sensitive if the data is string. |
### Examples
```csharp
[C#]
GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)
[VB]
GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)
```
### See Also
* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## Sort(int, int, int, int, int[]) {#sort_2}
Sorts the datas ascend top to bottom in a range of a WebWorksheet by some field that are specifed by column indexes array.
```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | The row number of the first cell to sort. |
| startColumn | Int32 | The column number of the first cell to sort. |
| rows | Int32 | Number of rows to be imported. |
| columns | Int32 | Number of columns to be imported. |
| indexes | Int32[] | The column indexes array that specifies the data sorted by. |
### Examples
```csharp
[C#]
int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);
[VB]
Dim indexes() As Integer =  New Integer(3) {}
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)
```
### See Also
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}
Sorts the datas ascend in a range of a WebWorksheet by some field that are specifed by indexes array.
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
| indexes | Int32[] | The column(or row) index that specifis the sort column(or row). If sort orientation is top to bottom, the index represents column index. If sort orientation is left to right, the index represents row index. |
| orders | SortByOrder[] | The sort order:Ascending or Descending |
| orientation | SortOrientation | The sort orientation: top to bottom or left to right. |
| isCaseSensitive | Boolean | Indicates whether the sorting is case sensitive. |
### Remarks
If you use this method to sort a block of data, please be sure that length of the parameter indexes equals length of the parameter orders.
### Examples
```csharp
```
[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)
### See Also
* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
