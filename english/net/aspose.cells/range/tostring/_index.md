---
title: Range.ToString
second_title: Aspose.Cells for .NET API Reference
description: Range method. Returns a string represents the current Range object
type: docs
url: /net/aspose.cells/range/tostring/
---
## Range.ToString method

Returns a string represents the current Range object.

```csharp
public override string ToString()
```

### Examples

```csharp
// Called: Console.WriteLine(workbook.Worksheets[0].Cells.MaxDisplayRange.ToString());
[Test]
        public void Method_ToString()
        {


            Aspose.Cells.HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ExportWorksheetCSSSeparately = true;
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
            htmlSaveOptions.LinkTargetType = HtmlLinkTargetType.Blank;
            htmlSaveOptions.DisableDownlevelRevealedComments = true;
            htmlSaveOptions.ExportImagesAsBase64 = false;//it was not worked before 20.3
            htmlSaveOptions.ExportActiveWorksheetOnly = true;
            htmlSaveOptions.HiddenColDisplayType = HtmlHiddenColDisplayType.Remove;
            htmlSaveOptions.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Remove;

            using (Aspose.Cells.Workbook workbook = new Aspose.Cells.Workbook(Constants.sourcePath + "NET48056.xlsm"))
            {
                workbook.Worksheets.ActiveSheetIndex = 0;
                Console.WriteLine(workbook.Worksheets[0].Cells.MaxDisplayRange.ToString());

                System.Diagnostics.Stopwatch sw = System.Diagnostics.Stopwatch.StartNew();
                workbook.Save(Constants.destPath + "NET48056.html", htmlSaveOptions);
                sw.Stop();
                Assert.LessOrEqual(sw.Elapsed.TotalSeconds, 15);
            }
            Workbook w = new Workbook(Constants.destPath + "NET48056.html");
            Assert.AreEqual("Prev. Employer - 2", w.Worksheets[0].Cells["J62"].StringValue, "Prev. Employer - 2");
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


