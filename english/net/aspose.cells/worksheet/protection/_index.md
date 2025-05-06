---
title: Worksheet.Protection
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version
type: docs
url: /net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Represents the various types of protection options available for a worksheet. Supports advanced protection options in ExcelXP and above version.

```csharp
public Protection Protection { get; }
```

### Remarks

This property can protect worksheet in all versions of Excel file and support advanced protection options in ExcelXP and above version.

### Examples

```csharp
// Called: Assert.IsTrue(sheet.Protection.AllowFiltering);
[Test]
        public void Property_Protection()
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

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


