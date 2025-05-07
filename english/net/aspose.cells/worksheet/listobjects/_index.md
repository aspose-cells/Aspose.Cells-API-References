---
title: Worksheet.ListObjects
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets all ListObjects in this worksheet
type: docs
url: /net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Gets all ListObjects in this worksheet.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Examples

```csharp
// Called: ListObject lo = workbook.Worksheets[0].ListObjects[0];
[Test]
        public void Property_ListObjects()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-54247/Template.xlsx");
            ListObject lo = workbook.Worksheets[0].ListObjects[0];
            lo.Resize(1, 0, 20, lo.EndColumn, true);
            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual("=SUBTOTAL(104,[Formula])", cells["M21"].Formula);
            Assert.AreEqual(BackgroundType.Solid, cells["H4"].GetStyle().Pattern);
            workbook.Save(Constants.destPath + "CellsNet54247.xlsx");
        }
```

### See Also

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


