---
title: ImageOrPrintOptions.DefaultFont
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. When characters in the Excel are Unicode and not be set with correct font in cell style They may appear as block in pdfimage. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set Aspose.Cells will use system default font to show these unicode characters
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```csharp
public string DefaultFont { get; set; }
```

### Examples

```csharp
// Called: imgOption.DefaultFont = "SimSun";
private void Property_DefaultFont(string filePath, string savePath, string fileName)
        {
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            loadOptions.Region = CountryCode.USA;
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;
            Workbook excel = new Workbook(filePath + fileName, loadOptions);
            excel.AcceptAllRevisions();

            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            saveOptions.ExportHiddenWorksheet = false;
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden;
            saveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;
            saveOptions.LinkTargetType = HtmlLinkTargetType.Blank;

            int sheetCount = excel.Worksheets.Count;
            // int visibleCount = 0;
            int originActiveIndex = excel.Worksheets.ActiveSheetIndex;
            Worksheet worksheet = null;

            Workbook checkExcel = GetCheckExcelLandRay(new FileStream(filePath + fileName, FileMode.Open, FileAccess.ReadWrite));
            bool canApplyStyle = CanApplyStyleLandRay(savePath, checkExcel, saveOptions);
            for (int i = 1; i <= sheetCount; i++)
            {
                worksheet = checkExcel.Worksheets[i - 1];
                Cells cells1 = worksheet.Cells;
                Cell cell1 = cells1["A6"];
                Style style1 = cell1.GetStyle();
                if (worksheet != null && worksheet.IsVisible)
                {
                    // visibleCount++;
                    excel.Worksheets.ActiveSheetIndex = i - 1;
                    if (canApplyStyle)
                    {
                        Style newStyle = checkExcel.CreateStyle();
                        newStyle.IsTextWrapped = true;
                        StyleFlag flag = new StyleFlag();
                        flag.WrapText = true;
                        newStyle.IsTextWrapped = true;
                        Cells cells = worksheet.Cells;
                        cells.ApplyStyle(newStyle, flag);
                    }
                    Cells cells2 = worksheet.Cells;
                    Cell cell2 = cells2["A6"];
                    Style style2 = cell2.GetStyle();
                    if (originActiveIndex == i - 1)
                    {
                        worksheet.PageSetup.PrintArea = "A1:I4";
                        ImageOrPrintOptions imgOption = new ImageOrPrintOptions();
                        imgOption.HorizontalResolution = 96;
                        imgOption.VerticalResolution = 96;
                        imgOption.DefaultFont = "SimSun";
                        imgOption.Quality = 100;
                        imgOption.OutputBlankPageWhenNothingToPrint = true;
                        imgOption.ImageType = ImageType.Png;
                        SheetRender sheetRender = new SheetRender(worksheet, imgOption);
                        sheetRender.ToImage(0, savePath + "thumbnail.png");
                    }
                    excel.Save(savePath + "pageResult" + i + ".html", saveOptions);
                }
            }
        }
```

### See Also

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


