---
title: PdfSaveOptions.PdfSaveOptions
second_title: Aspose.Cells for .NET API Reference
description: PdfSaveOptions constructor. Creates the options for saving pdf file
type: docs
url: /net/aspose.cells/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Creates the options for saving pdf file.

```csharp
public PdfSaveOptions()
```

### Examples

```csharp
// Called: PdfSaveOptions options = new PdfSaveOptions();
[Test]
        public void PdfSaveOptions_Constructor()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET45037_&quot;;
            Workbook wb = new Workbook(filePath + &quot;pivot+table+sample.xlsx&quot;);
            wb.Settings.GlobalizationSettings.PivotSettings = new CustomGlobalPolish();
            PivotTable pt = wb.Worksheets[1].PivotTables[0];
            pt.RefreshData();
            pt.CalculateData();
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;
            wb.Save(CreateFolder(filePath) + &quot;out_polish.xlsx&quot;);
            Assert.AreEqual(wb.Worksheets[1].Cells[&quot;A5&quot;].StringValue, &quot;Suma końcowa&quot;);
            Assert.AreEqual(wb.Worksheets[1].Cells[&quot;D2&quot;].StringValue, &quot;Suma końcowa&quot;);
            Assert.AreEqual(wb.Worksheets[1].Cells[&quot;A4&quot;].StringValue, &quot;80101 Suma&quot;);

         

            wb = new Workbook(filePath + &quot;pivot_en.xlsx&quot;);
            wb.Settings.GlobalizationSettings.PivotSettings = new CustomGlobalChinese();
            pt = wb.Worksheets[0].PivotTables[0];
            pt.DataFields[0].DisplayName = &quot;乘积项:e&quot;;
            pt.DataFields[1].DisplayName = &quot;求和项:g&quot;;
            //pt.RefreshData();
            pt.CalculateData();
            wb.Save(Constants.PivotTableDestPath + &quot;NET45037.xlsx&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B11&quot;].StringValue, &quot;(全部)&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;B12&quot;].StringValue, &quot;(全部)&quot;);

            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;C14&quot;].StringValue, &quot;列标签&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A16&quot;].StringValue, &quot;行标签&quot;);

            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A18&quot;].StringValue, &quot;aa 求和&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A27&quot;].StringValue, &quot;(空白)&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A28&quot;].StringValue, &quot;(空白) 求和&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;A29&quot;].StringValue, &quot;总计&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;C16&quot;].StringValue, &quot;乘积项:e&quot;);
            Assert.AreEqual(wb.Worksheets[0].Cells[&quot;D16&quot;].StringValue, &quot;求和项:g&quot;);

            wb.Worksheets[0].AutoFitColumns();
            wb.Save(CreateFolder(filePath) + &quot;out_chinese.pdf&quot;);
        }
```

### See Also

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


