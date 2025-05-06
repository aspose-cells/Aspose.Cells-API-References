---
title: PageSetup.PrintCopies
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Get and sets number of copies to print
type: docs
url: /net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Get and sets number of copies to print.

```csharp
public int PrintCopies { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].PageSetup.PrintCopies, 1);
[Test]
        public void Property_PrintCopies()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet43062.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.PrintCopies, 1);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


