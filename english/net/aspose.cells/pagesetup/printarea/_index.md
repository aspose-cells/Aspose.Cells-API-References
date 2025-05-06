---
title: PageSetup.PrintArea
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the range to be printed
type: docs
url: /net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Represents the range to be printed.

```csharp
public string PrintArea { get; set; }
```

### Examples

```csharp
// Called: worksheet.PageSetup.PrintArea = range.Address;
[Test]
        public void Property_PrintArea()
        {
            Workbook wbc = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet565759.xlsx&quot;);
            wbc.Worksheets.RefreshPivotTables();
            var range = wbc.Worksheets.GetRangeByName(&quot;To_Publish&quot;);
            var worksheet = range.Worksheet;
            worksheet.PageSetup.PrintArea = range.Address;
            Assert.AreEqual(&quot;A1:B1&quot;, worksheet.PageSetup.PrintArea);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


