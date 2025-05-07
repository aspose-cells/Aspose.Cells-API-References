---
title: CellArea.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the end column of this area
type: docs
url: /net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Gets or set the end column of this area.

```csharp
public int EndColumn;
```

### Examples

```csharp
// Called: cellArea.EndColumn = 1;
[Test]
        public void Field_EndColumn()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "FindStringContains.xls");
            Worksheet grid = workbook.Worksheets[0];
            Cell foundCell = null;

            CellArea cellArea = new CellArea();
            cellArea.StartRow = 0;
            cellArea.EndRow = 1;
            cellArea.StartColumn = 0;
            cellArea.EndColumn = 1;
            FindOptions options = new FindOptions();
            options.LookAtType = LookAtType.Contains;
            options.CaseSensitive = false;
            foundCell = grid.Cells.Find("Test", foundCell, options);
            Assert.AreEqual(foundCell.Name, "A1");

        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


