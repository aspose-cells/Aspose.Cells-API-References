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
// Called: Assert.IsTrue(sheet.Protection.AllowFormattingColumn);
[Test]
        public void Property_Protection()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45683.xml");
            Worksheet sheet = workbook.Worksheets["Cars (1)"];
            Assert.IsTrue(sheet.Protection.AllowDeletingRow);
            Assert.IsTrue(sheet.Protection.AllowSorting);
            Assert.IsTrue(sheet.Protection.AllowFiltering);
            Assert.IsTrue(sheet.Protection.AllowFormattingColumn);
            workbook.Save(Constants.destPath + "CellsNet45683.xml");
            workbook = new Workbook(Constants.destPath + "CellsNet45683.xml");
            sheet = workbook.Worksheets["Cars (1)"];
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


