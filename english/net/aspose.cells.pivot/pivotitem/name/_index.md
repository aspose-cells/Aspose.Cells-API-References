---
title: PivotItem.Name
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets the name of the pivot item
type: docs
url: /net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Gets the name of the pivot item.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Sum of d",workbook.Worksheets[0].PivotTables[0].RowFields[1].PivotItems[0].Name);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "NET46810_a.xlsx");
            Assert.AreEqual("Sum of d",workbook.Worksheets[0].PivotTables[0].RowFields[1].PivotItems[0].Name);
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


