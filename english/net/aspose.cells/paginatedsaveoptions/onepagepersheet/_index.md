---
title: PaginatedSaveOptions.OnePagePerSheet
second_title: Aspose.Cells for .NET API Reference
description: PaginatedSaveOptions property. If OnePagePerSheet is true  all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid and the other settings of pagesetup will still take effect
type: docs
url: /net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Examples

```csharp
// Called: options.OnePagePerSheet = true;
[Test]
        public void Property_OnePagePerSheet()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET47301_&quot;;
            Workbook wb = new Workbook(filePath + &quot;Gross Profit.xlsx&quot;);

            Worksheet sheet = wb.Worksheets[0];
            PivotTableCollection tables = sheet.PivotTables;
            for (int i = 0; i &lt; tables.Count; i++)
            {
                PivotTable pt = tables[i];
                pt.RefreshData();
                pt.CalculateData();
                // Get name
                string name = pt.Name;
                // Get image
                int startRow = pt.TableRange2.StartRow + 1;
                int endRow = pt.TableRange2.EndRow + 1;
                int startColumn = pt.TableRange2.StartColumn;
                int endColumn = pt.TableRange2.EndColumn;

                string upperLeftName = CellsHelper.CellIndexToName(startRow, startColumn);
                string lowerRightName = CellsHelper.CellIndexToName(endRow, endColumn);
                byte[] image = CreateImageFromRange(sheet, upperLeftName, lowerRightName);

                System.IO.File.WriteAllBytes(CreateFolder(filePath) + i.ToString() + &quot;-output.png&quot;, image);

            }

            Assert.AreEqual(sheet.Cells[&quot;M4&quot;].StringValue, &quot;2018&quot;);
            Assert.AreEqual(sheet.Cells[&quot;N4&quot;].StringValue, &quot;2019&quot;);
            Assert.AreEqual(sheet.Cells[&quot;M29&quot;].StringValue, &quot;2018&quot;);
            Assert.AreEqual(sheet.Cells[&quot;N29&quot;].StringValue, &quot;2019&quot;);

            Assert.AreEqual(sheet.Cells[&quot;Q4&quot;].StringValue, &quot;2018&quot;);
            Assert.AreEqual(sheet.Cells[&quot;R4&quot;].StringValue, &quot;2019&quot;);
            Assert.AreEqual(sheet.Cells[&quot;Q29&quot;].StringValue, &quot;2018&quot;);
            Assert.AreEqual(sheet.Cells[&quot;R29&quot;].StringValue, &quot;2019&quot;);

            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;
            sheet.PageSetup.PrintArea = &quot;&quot;;
            wb.Save(CreateFolder(filePath) + &quot;out.pdf&quot;, options);
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


