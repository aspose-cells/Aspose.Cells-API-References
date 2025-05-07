---
title: Worksheet.AutoFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents auto filter for the specified worksheet
type: docs
url: /net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Represents auto filter for the specified worksheet.

```csharp
public AutoFilter AutoFilter { get; }
```

### Examples

```csharp
// Called: worksheet.AutoFilter.FilterTop10(5, true, false, 5);
[Test]
        public void Property_AutoFilter()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46029.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "B6:K6";
            worksheet.AutoFilter.Custom(4, FilterOperatorType.GreaterThan, 500);
            worksheet.AutoFilter.Refresh();
            Assert.IsTrue(worksheet.Cells.IsRowHidden(7));
            workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46029.xlsx");
            worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "B6:K6";
            worksheet.AutoFilter.Custom(5, FilterOperatorType.Equal, "", false, FilterOperatorType.GreaterThan, 500); 
            worksheet.AutoFilter.Refresh();
            Assert.IsFalse(worksheet.Cells.IsRowHidden(13));
            workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46029.xlsx");
            worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "B6:K6";
            worksheet.AutoFilter.FilterTop10(5, false, false, 5); 
            worksheet.AutoFilter.Refresh();
            Assert.IsTrue(worksheet.Cells.IsRowHidden(13));
            workbook = new Workbook(Constants.sourcePath + "AutoFilter/CellsNet46029.xlsx");
            worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "B6:K6";
            worksheet.AutoFilter.FilterTop10(5, true, false, 5);
            worksheet.AutoFilter.Refresh();
            Assert.IsTrue(worksheet.Cells.IsRowHidden(13));
        }
```

### See Also

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


