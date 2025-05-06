---
title: Workbook.AcceptAllRevisions
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Accepts all tracked changes in the workbook
type: docs
url: /net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Accepts all tracked changes in the workbook.

```csharp
public void AcceptAllRevisions()
```

### Examples

```csharp
// Called: excel.AcceptAllRevisions();
[Test]
        public void Method_AcceptAllRevisions()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;JAVA42944/&quot;;

            string savePath = CreateFolder(filePath);
            string fileName = &quot;无宏转换失败.xlsx&quot;;

            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = &quot;SimSun&quot;;
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

            Workbook checkExcel = getCheckExcel42944(new FileStream(filePath + fileName, FileMode.Open, FileAccess.ReadWrite));
            bool canApplyStyle = canApplyStyle42944(savePath, checkExcel, saveOptions);
            for (int i = 1; i &lt;= sheetCount; i++)
            {
                worksheet = checkExcel.Worksheets[i - 1];
                Cells cells1 = worksheet.Cells;
                Cell cell1 = cells1[&quot;A6&quot;];
                Style style1 = cell1.GetStyle();
                if (worksheet != null &amp;&amp; worksheet.IsVisible)
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
                    Cell cell2 = cells2[&quot;A6&quot;];
                    Style style2 = cell2.GetStyle();
                    if (originActiveIndex == i - 1)
                    {
                        worksheet.PageSetup.PrintArea = &quot;A1:I4&quot;;
                        ImageOrPrintOptions imgOption = new ImageOrPrintOptions();
                        imgOption.HorizontalResolution = 96;
                        imgOption.VerticalResolution = 96;
                        imgOption.DefaultFont = &quot;SimSun&quot;;
                        imgOption.Quality = 100;
                        imgOption.OutputBlankPageWhenNothingToPrint = true;
                        imgOption.ImageType = ImageType.Png;
                        SheetRender sheetRender = new SheetRender(worksheet, imgOption);
                        sheetRender.ToImage(0, savePath + &quot;thumbnail.png&quot;);
                    }
                    excel.Save(savePath + &quot;pageResult&quot; + i + &quot;.html&quot;, saveOptions);
                }
            }
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


