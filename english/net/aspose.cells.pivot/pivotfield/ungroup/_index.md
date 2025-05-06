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
// Called: pt.ColumnFields[0].Ungroup();
[Test]
        public void Method_Ungroup()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet54443.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.ColumnFields[0].Ungroup();
            Assert.AreEqual(1, pt.ColumnFields.Count);
            Assert.AreEqual(&quot;1&quot;, workbook.Worksheets[0].Cells[&quot;H8&quot;].StringValue);

            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;CellsNet54443_1.xlsx&quot;);

        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


