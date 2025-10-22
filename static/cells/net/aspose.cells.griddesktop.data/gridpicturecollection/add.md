##GridPictureCollection.Add
GridPictureCollection method. Adds a picture to the collection
## Add(int, int, int, int, Stream) {#add}
Adds a picture to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn,
Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| lowerRightRow | Int32 | Lower right row index |
| lowerRightColumn | Int32 | Lower right column index |
| stream | Stream | Stream object which contains the image data. |
### Return Value
Picture object index.
### See Also
* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int, int, int, string) {#add_1}
Adds a picture to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn,
string fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| lowerRightRow | Int32 | Lower right row index |
| lowerRightColumn | Int32 | Lower right column index |
| fileName | String | Image filename. |
### Return Value
Picture object index.
### See Also
* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int, Stream) {#add_2}
Adds a picture to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| stream | Stream | Stream object which contains the image data. |
### Return Value
Picture object index.
### See Also
* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int, string) {#add_3}
Adds a picture to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| fileName | String | Image filename. |
### Return Value
[`GridPicture`](../../gridpicture/) object index.
### See Also
* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int, string, int, int) {#add_4}
Adds a picture to the collection.
```csharp
public int Add(int upperLeftRow, int upperLeftColumn, string fileName, int widthScale,
int heightScale)
```
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| fileName | String | Image filename. |
| widthScale | Int32 | Scale of image width, a percentage. |
| heightScale | Int32 | Scale of image height, a percentage. |
### Return Value
[`GridPicture`](../../gridpicture/) object index.
### See Also
* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(string, string) {#add_6}
Adds a Picture to a specified cell by cell name.
```csharp
public void Add(string cellName, string fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Name of grid cell. |
| fileName | String | File name of picture. |
### See Also
* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## Add(int, int, Image) {#add_5}
Adds a Picture to a specified cell at row column index.
```csharp
public void Add(int row, int col, Image image)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index of cell. |
| col | Int32 | Column index of cell. |
| image | Image | Image. |
### See Also
* class [GridPictureCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
