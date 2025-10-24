##GridSheetRender.ToTiff
GridSheetRender method. Render whole worksheet as Tiff Image to stream
## ToTiff(Stream) {#totiff}
Render whole worksheet as Tiff Image to stream.
```csharp
public void ToTiff(Stream stream)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | the stream of the output image |
### See Also
* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
## ToTiff(string) {#totiff_1}
Render whole worksheet as Tiff Image to a file.
```csharp
public void ToTiff(string filename)
```
| Parameter | Type | Description |
| --- | --- | --- |
| filename | String | the filename of the output image |
### Examples
The following code outputs all the pages of the first sheet to Tiff image.
```csharp
//load the source file with images.
Workbook wb = new Workbook("Book1.xlsx");
ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
//set output image type.
imgOpt.SaveFormat = SaveFormat.Tiff;
//render the first sheet.
SheetRender sr = new SheetRender(wb.Worksheets[0], imgOpt);
//output all the pages of the sheet to Tiff image.
sr.ToTiff("output.tiff");
```
### See Also
* class [GridSheetRender](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)
