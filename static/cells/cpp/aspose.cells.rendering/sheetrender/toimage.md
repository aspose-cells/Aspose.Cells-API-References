##Aspose::Cells::Rendering::SheetRender::ToImage method
'Aspose::Cells::Rendering::SheetRender::ToImage method. Render certain page to a file in C++.'
## SheetRender::ToImage(int32_t, const U16String\&) method
Render certain page to a file.
```cpp
void Aspose::Cells::Rendering::SheetRender::ToImage(int32_t pageIndex, const U16String &fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int32_t | indicate which page is to be converted |
| fileName | const U16String\& | filename of the output image |
## Examples
```cpp
Aspose::Cells::Startup();
//The following code outputs the first page of the first sheet to png image.
//load the source file with images.
Workbook wb(u"Book1.xlsx");
ImageOrPrintOptions imgOpt;
//set output image type.
imgOpt.SetImageType(ImageType::Png);
//render the first sheet.
SheetRender sr(wb.GetWorksheets().Get(0), imgOpt);
//output the first page of the sheet to image.
U16String val =  u"output.png";
sr.ToImage(0, val);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [U16String](../../../aspose.cells/u16string/)
* Class [SheetRender](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
## SheetRender::ToImage(int32_t, const char16_t*) method
Render certain page to a file.
```cpp
void Aspose::Cells::Rendering::SheetRender::ToImage(int32_t pageIndex, const char16_t *fileName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int32_t | indicate which page is to be converted |
| fileName | const char16_t* | filename of the output image |
## Examples
```cpp
Aspose::Cells::Startup();
//The following code outputs the first page of the first sheet to png image.
//load the source file with images.
Workbook wb(u"Book1.xlsx");
ImageOrPrintOptions imgOpt;
//set output image type.
imgOpt.SetImageType(ImageType::Png);
//render the first sheet.
SheetRender sr(wb.GetWorksheets().Get(0), imgOpt);
//output the first page of the sheet to image.
sr.ToImage(0, u"output.png");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetRender](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
## SheetRender::ToImage(int32_t) method
Render certain page to a stream.
```cpp
Vector<uint8_t> Aspose::Cells::Rendering::SheetRender::ToImage(int32_t pageIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pageIndex | int32_t | indicate which page is to be converted |
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [SheetRender](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
