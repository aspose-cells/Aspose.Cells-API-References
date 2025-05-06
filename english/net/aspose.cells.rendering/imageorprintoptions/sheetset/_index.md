---
title: ImageOrPrintOptions.SheetSet
second_title: Aspose.Cells for .NET API Reference
description: ImageOrPrintOptions property. Gets or sets the sheets to render. Default is all visible sheets in the workbook Visible
type: docs
url: /net/aspose.cells.rendering/imageorprintoptions/sheetset/
---
## ImageOrPrintOptions.SheetSet property

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [`Visible`](../../sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Remarks

The set is ignored when it is used in [`SheetRender`](../../sheetrender/)

### Examples

```csharp
// Called: imgOpt.SheetSet = SheetSet.All;
[Test]
        public void Property_SheetSet()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-51597.xlsx&quot;);

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.SheetSet = SheetSet.Visible;
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, pdfSaveOptions);
                ms.Position = 0;
                using (StreamReader reader = new StreamReader(ms))
                {
                    string content = reader.ReadToEnd();
                    Regex regex = new Regex(@&quot;/Count\s*(\d+)&quot;);
                    Assert.AreEqual(&quot;9&quot;, regex.Match(content).Groups[1].Value);
                }
            }

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.SheetSet = SheetSet.All;
            Assert.AreEqual(11, new WorkbookPrintingPreview(wb, imgOpt).EvaluatedPageCount);

            int hiddenSheetIndex = 3;
            imgOpt.SheetSet = new SheetSet(new int[] { hiddenSheetIndex });
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            Assert.AreEqual(2, wr.PageCount);
            using (MemoryStream ms = new MemoryStream())
            {
                wr.ToImage(0, ms);
                Assert.IsTrue(ms.Length &gt; 0);
            }

            //Hidden sheet is not output in SheetRender.
            SheetRender sr = new SheetRender(wb.Worksheets[hiddenSheetIndex], new ImageOrPrintOptions());
            Assert.AreEqual(0, sr.PageCount);
            using (MemoryStream ms = new MemoryStream())
            {
                sr.ToImage(0, new MemoryStream());
                Assert.AreEqual(0, ms.Length);
            }


            imgOpt.SheetSet = new SheetSet(new int[] { 1, 3 });
            Assert.AreEqual(5, new WorkbookRender(wb, imgOpt).PageCount);
            Assert.AreEqual(5, new WorkbookPrintingPreview(wb, imgOpt).EvaluatedPageCount);
        }
```

### See Also

* class [SheetSet](../../sheetset/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


