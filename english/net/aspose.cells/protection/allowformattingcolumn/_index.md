---
title: Protection.AllowFormattingColumn
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the formatting of columns is allowed on a protected worksheet
type: docs
url: /net/aspose.cells/protection/allowformattingcolumn/
---
## Protection.AllowFormattingColumn property

Represents if the formatting of columns is allowed on a protected worksheet

```csharp
public bool AllowFormattingColumn { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(sheet.Protection.AllowFormattingColumn);
[Test]
        public void Property_AllowFormattingColumn()
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

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


