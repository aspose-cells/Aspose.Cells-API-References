---
title: PasteOptions.OnlyVisibleCells
second_title: Aspose.Cells for .NET API Reference
description: PasteOptions property. True means only copying visible cells
type: docs
url: /net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True means only copying visible cells.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Examples

```csharp
// Called: pasteOptions.OnlyVisibleCells = true;
[Test]
        public void Property_OnlyVisibleCells()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("a");
            cells["C3"].PutValue("b");
            cells.HideColumn(1);
            cells.HideRow(1);
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:C3");
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            destRange.Copy(sourceRange, pasteOptions);
            Assert.AreEqual(destCells["B2"].StringValue, "b");
        }
```

### See Also

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


