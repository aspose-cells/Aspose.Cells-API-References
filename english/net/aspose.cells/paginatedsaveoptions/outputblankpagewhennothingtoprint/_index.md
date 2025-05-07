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
            string filePath = Constants.PivotTableSourcePath + @"NETCORE94_";
            string savePath = CreateFolder(filePath);

            // Creating a file stream containing the Excel file to be opened
            FileStream excelStream = new FileStream(filePath + @"AsposeCellsTestFile.xlsx", FileMode.Open, FileAccess.Read);

            // Instantiate a Workbook object that represents the existing Excel file
            Workbook workbook = new Workbook(excelStream);

            Worksheet wkInput = workbook.Worksheets["input"];
            wkInput.Cells["B2"].Value = 2936;
            //wkInput.Cells["A1068"].Value = 44083.625;
            //wkInput.Cells["A1068"].Value = "9/9/2020  15:00:00 PM";
            //wkInput.Cells["B1068"].Value = 1111;

            foreach (Worksheet workSheet in workbook.Worksheets)
            {
                if (workSheet.PivotTables.Count < 1)
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
            workbook.Save(savePath + @"out.pdf", options);
            workbook.Save(savePath + @"out.xlsx");
            Assert.AreEqual(workbook.Worksheets["pivot"].Cells["B5"].StringValue, "<9/5/2020");
            Assert.AreEqual(workbook.Worksheets["pivot"].Cells["B6"].StringValue, "5-Sep");
           

            excelStream.Close();
            excelStream.Dispose();
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


