---
title: PivotField.Ungroup
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Ungroup the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Ungroup the pivot field.

```csharp
public void Ungroup()
```

### Examples

```csharp
// Called: pt.RowFields[0].Ungroup();
[Test]
        public void Method_Ungroup()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CellsNet54443.xlsx");
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.RowFields[0].Ungroup();
            Assert.AreEqual(1, pt.RowFields.Count);
            Assert.AreEqual("10/19/2023", workbook.Worksheets[0].Cells["G9"].StringValue);

            workbook.Save(Constants.PivotTableDestPath + "CellsNet54443.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


