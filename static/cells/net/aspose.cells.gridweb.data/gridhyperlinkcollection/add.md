##GridHyperlinkCollection.Add
GridHyperlinkCollection method. Adds a hyperlink to a specified cell or a range of cells
## Add(int, int, int, int, string) {#add}
Adds a hyperlink to a specified cell or a range of cells.
```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of the hyperlink range. |
| firstColumn | Int32 | First column of the hyperlink range. |
| totalRows | Int32 | Number of rows in this hyperlink range. |
| totalColumns | Int32 | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |
### Return Value
[`GridHyperlink`](../../gridhyperlink/) object index.
### See Also
* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## Add(string, int, int, string) {#add_1}
Adds a hyperlink to a specified cell or a range of cells.
```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| totalRows | Int32 | Number of rows in this hyperlink range. |
| totalColumns | Int32 | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |
### Return Value
[`GridHyperlink`](../../gridhyperlink/) object index.
### See Also
* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## Add(string, string) {#add_2}
Adds a hyperlink to a specified cell .
```csharp
public int Add(string cellName, string address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| address | String | Address of the hyperlink. |
### Return Value
[`GridHyperlink`](../../gridhyperlink/) object index.
### See Also
* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
## Add(string, string, string, string, string) {#add_3}
Adds a hyperlink to a specified cell or a range of cells.
```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay,
string screenTip)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |
### Return Value
[`GridHyperlink`](../../gridhyperlink/) object index.
### See Also
* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)
