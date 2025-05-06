---
title: PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. Indicates whether to output a blank page when there is nothing to print
type: docs
url: /net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Indicates whether to output a blank page when there is nothing to print.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Remarks

Default is true.

### Examples

```csharp
// Called: OutputBlankPageWhenNothingToPrint = false,
[Test]
        public void Property_OutputBlankPageWhenNothingToPrint()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NETCORE94_&quot;;
            string savePath = CreateFolder(filePath);

            // Creating a file stream containing the Excel file to be opened
            FileStream excelStream = new FileStream(filePath + @&quot;AsposeCellsTestFile.xlsx&quot;, FileMode.Open, FileAccess.Read);

            // Instantiate a Workbook object that represents the existing Excel file
            Workbook workbook = new Workbook(excelStream);

            Worksheet wkInput = workbook.Worksheets[&quot;input&quot;];
            wkInput.Cells[&quot;B2&quot;].Value = 2936;
            //wkInput.Cells[&quot;A1068&quot;].Value = 44083.625;
            //wkInput.Cells[&quot;A1068&quot;].Value = &quot;9/9/2020  15:00:00 PM&quot;;
            //wkInput.Cells[&quot;B1068&quot;].Value = 1111;

            foreach (Worksheet workSheet in workbook.Worksheets)
            {
                if (workSheet.PivotTables.Count &lt; 1)
                {
                    workSheet.IsVisible = false;
                }
                else
                {
                    PivotTable pivotTable = workSheet.PivotTables[0];
                    //pivotTable.RefreshDataFlag = true;
                    pivotTable.PreserveFormatting = true;
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                    pivotTable.RefreshData();
                    //pivotTable.RefreshDataFlag = false;
                    //workSheet.RefreshPivotTables();
                    workSheet.PageSetup.SetFitToPages(1, 0);
                    workSheet.AutoFitRows();
                }
            }


            PdfSaveOptions options = new PdfSaveOptions()
            {
                CreatedTime = DateTime.Now,
                CalculateFormula = true,
                //ImageType = ImageType.OfficeCompatibleEmf,
                OutputBlankPageWhenNothingToPrint = false,
                RefreshChartCache = true,
                AllColumnsInOnePagePerSheet = true
            };
            workbook.Save(savePath + @&quot;out.pdf&quot;, options);
            workbook.Save(savePath + @&quot;out.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[&quot;pivot&quot;].Cells[&quot;B5&quot;].StringValue, &quot;&lt;9/5/2020&quot;);
            Assert.AreEqual(workbook.Worksheets[&quot;pivot&quot;].Cells[&quot;B6&quot;].StringValue, &quot;5-Sep&quot;);
           

            excelStream.Close();
            excelStream.Dispose();
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


