##Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method
'Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
## ImageOrPrintOptions::SetHorizontalResolution method
Gets or sets the horizontal resolution for generated images, in dots per inch.
```cpp
void Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution(int32_t value)
```
## Remarks
The default value is 96.
Setting HorizontalResolution and VerticalResolution effects the width and height of the output image in pixels.
## Examples
```cpp
Aspose::Cells::Startup();
//          The following code sets resolution to 192, the width and height of the generated image is twice of
//          the one with resolution left as the default value 96.
Workbook wb(u"Book1.xlsx");
ImageOrPrintOptions opts;
//Set output image type: png.
opts.SetImageType(ImageType::Png);
//Set resolution to 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);
//Render worksheet page to image.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
