---
title: Protection.AllowSorting
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the sorting option is allowed on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowsorting/
---
## Protection.AllowSorting property

Represents if the sorting option is allowed on a protected worksheet.

```csharp
public bool AllowSorting { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(sheet.Protection.AllowSorting);
[Test]
        public void Property_AllowSorting()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45683.xml&quot;);
            Worksheet sheet = workbook.Worksheets[&quot;Cars (1)&quot;];
            Assert.IsTrue(sheet.Protection.AllowDeletingRow);
            Assert.IsTrue(sheet.Protection.AllowSorting);
            Assert.IsTrue(sheet.Protection.AllowFiltering);
            Assert.IsTrue(sheet.Protection.AllowFormattingColumn);
            workbook.Save(Constants.destPath + &quot;CellsNet45683.xml&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet45683.xml&quot;);
            sheet = workbook.Worksheets[&quot;Cars (1)&quot;];
            Assert.IsTrue(sheet.Protection.AllowDeletingRow);
            Assert.IsTrue(sheet.Protection.AllowSorting);
            Assert.IsTrue(sheet.Protection.AllowFiltering);
            Assert.IsTrue(sheet.Protection.AllowFormattingColumn);
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


