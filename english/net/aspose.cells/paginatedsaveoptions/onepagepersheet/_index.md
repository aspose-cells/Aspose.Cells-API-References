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
            string filePath = Constants.PivotTableSourcePath + @"JAVA40251_";
            Workbook wb = new Workbook(filePath + "ARTIF_exhibits.xlsx");
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;
            Worksheet sheet = wb.Worksheets["GICS Sector Exposure"];
            Cells cells = sheet.Cells;
            Cell b6 = cells["B6"];
            Cell b7 = cells["B7"];
            Assert.AreEqual(b6.GetStyle().HorizontalAlignment, TextAlignmentType.Center);
            Assert.AreEqual(b6.GetStyle().IndentLevel, 0);

            Assert.AreEqual(b7.GetStyle().HorizontalAlignment, TextAlignmentType.Right);
            Assert.AreEqual(b7.GetStyle().IndentLevel, 2);

            sheet.PivotTables[0].CalculateData();

            Assert.AreEqual(b6.GetStyle().HorizontalAlignment, TextAlignmentType.Center);
            Assert.AreEqual(b6.GetStyle().IndentLevel, 0);

            Assert.AreEqual(b7.GetStyle().HorizontalAlignment, TextAlignmentType.Right);
            Assert.AreEqual(b7.GetStyle().IndentLevel, 2);

            wb.Save(CreateFolder(filePath) + "out.pdf", options);
        }
```

### See Also

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


