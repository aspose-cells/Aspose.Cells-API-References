---
title: WorksheetCollection.Dxfs
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the master differential formatting records
type: docs
url: /net/aspose.cells/worksheetcollection/dxfs/
---
## WorksheetCollection.Dxfs property

Gets the master differential formatting records.

```csharp
public DxfCollection Dxfs { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets.Dxfs.Count == 0);
[Test]
        public void Property_Dxfs()
        {
            var workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings/CellsNet47425.xlsx");

            var rule1 = workbook.Worksheets["Sheet1"].ConditionalFormattings[0];
            var priority1 = rule1[0].Priority;
            Assert.AreEqual(4, priority1);
            Assert.IsTrue(workbook.Worksheets.Dxfs.Count == 0);
        }
```

### See Also

* class [DxfCollection](../../dxfcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


