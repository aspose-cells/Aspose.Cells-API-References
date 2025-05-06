---
title: PivotTable.RowFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as row fields
type: docs
url: /net/aspose.cells.pivot/pivottable/rowfields/
---
## PivotTable.RowFields property

Returns a PivotFields object that are currently shown as row fields.

```csharp
public PivotFieldCollection RowFields { get; }
```

### Examples

```csharp
// Called: pt.RowFields[0].Ungroup();
[Test]
        public void Property_RowFields()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet54443.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.RowFields[0].Ungroup();
            Assert.AreEqual(1, pt.RowFields.Count);
            Assert.AreEqual(&quot;10/19/2023&quot;, workbook.Worksheets[0].Cells[&quot;G9&quot;].StringValue);

            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet54443.xlsx&quot;);
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


