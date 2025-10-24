##GridSheetRender.ToImage
GridSheetRender method. Render certain page to a Graphics
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}
Render certain page to a Graphics
```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |
| width | Single | The maximum width (in pixels) that can be occupied by the rendered page. |
| height | Single | The maximum height (in pixels) that can be occupied by the rendered page. |
### See Also
* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ToImage(int, Graphics, float, float) {#toimage_1}
Render certain page to a Graphics
```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| g | Graphics | The object where to render to. |
| x | Single | The X coordinate (in pixels) of the top left corner of the rendered page. |
| y | Single | The Y coordinate (in pixels) of the top left corner of the rendered page. |
### See Also
* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ToImage(int, string) {#toimage_4}
Render certain page to a file.
```csharp
public void ToImage(int pageIndex, string fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| fileName | String | filename of the output image |
### Examples
The following code outputs the first page of the first sheet to png image.
```csharp
//load the source file with images.
Workbook wb = new Workbook("Book1.xlsx");
ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
//set output image type.
imgOpt.ImageType = ImageType.Png;
//render the first sheet.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);
//output the first page of the sheet to image.
sr.ToImage(0, "output.png");
```
### See Also
* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ToImage(int, Stream) {#toimage_3}
Render certain page to a stream.
```csharp
public void ToImage(int pageIndex, Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
| stream | Stream | the stream of the output image |
### See Also
* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ToImage(int) {#toimage}
Render certain page to a Bitmap object.
```csharp
public Bitmap ToImage(int pageIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | Int32 | indicate which page is to be converted |
### Return Value
the bitmap object of the page
### See Also
* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
