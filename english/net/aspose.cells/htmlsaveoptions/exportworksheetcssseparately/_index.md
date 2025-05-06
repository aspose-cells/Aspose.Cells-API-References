---
title: HtmlSaveOptions.ExportWorksheetCSSSeparately
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. Indicating whether export the worksheet css separately.The default value is false
type: docs
url: /net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Indicating whether export the worksheet css separately.The default value is false.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Examples

```csharp
// Called: htmlSaveOptions.ExportWorksheetCSSSeparately = true;
[Test]
        public void Property_ExportWorksheetCSSSeparately()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET48435/&quot;;
            string inputFilePath = filePath + &quot;notificacoes 28-05-2021.xlsx&quot;;
            string savePath = CreateFolder(filePath);

            int activeSheetIndex = 1;//index is 0-based, so this is a 2nd worksheet

            Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ExportWorksheetCSSSeparately = true;
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
            htmlSaveOptions.DisableDownlevelRevealedComments = true;
            htmlSaveOptions.ExportImagesAsBase64 = false;//it was not worked before 20.3
            htmlSaveOptions.ExportActiveWorksheetOnly = true;

            htmlSaveOptions.MergeEmptyTdForcely = true;
            htmlSaveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            htmlSaveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;

            using (Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(inputFilePath))
            {
                workbook.Worksheets.ActiveSheetIndex = activeSheetIndex;

                System.Diagnostics.Stopwatch sw = System.Diagnostics.Stopwatch.StartNew();
                workbook.Save(savePath + &quot;out&quot; + activeSheetIndex + &quot;.html&quot;, htmlSaveOptions);
                sw.Stop();
                Assert.LessOrEqual(sw.Elapsed.Seconds, 20);
            }
        }
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


