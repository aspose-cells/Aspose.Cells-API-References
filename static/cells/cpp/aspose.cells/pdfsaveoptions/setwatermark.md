##Aspose::Cells::PdfSaveOptions::SetWatermark method
'Aspose::Cells::PdfSaveOptions::SetWatermark method. Gets or sets watermark to output in C++.'
## PdfSaveOptions::SetWatermark method
Gets or sets watermark to output.
```cpp
void Aspose::Cells::PdfSaveOptions::SetWatermark(const RenderingWatermark &value)
```
## Examples
```cpp
Aspose::Cells::Startup();
//The following code sets watermark in the output pdf.
//prepare a workbook with 3 pages.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);
//create a font for watermark, and specify bold, italic, color
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue
//create a watermark from text and the specified font
RenderingWatermark watermark(u"Watermark", font);
//specify horizontal and vertical alignment
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);
//specify rotation
watermark.SetRotation(30);
//specify opacity
watermark.SetOpacity(0.6f);
//specify the scale to page(e.g. 100, 50) in percent.
watermark.SetScaleToPagePercent(50);
//spcify watermark for rendering to pdf.
PdfSaveOptions options;
if (options.GetWatermark().IsNull())
{
options.SetWatermark(watermark);
}
wb.Save(u"output_watermark.pdf", options);
Aspose::Cells::Cleanup();
```
## See Also
* Class [Vector](../../vector/)
* Class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
