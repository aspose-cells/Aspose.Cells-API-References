---
title: PivotTable.ColumnFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a PivotFields object that are currently shown as column fields
type: docs
url: /net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Returns a PivotFields object that are currently shown as column fields.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Examples

```csharp
// Called: PivotField field = pivot.ColumnFields[0];
[Test]
        public void Property_ColumnFields()
        {
            Workbook book = AddNewWorkbok();
            PivotTable pivot = AddNewPivotTable(book);
            //Add PivotFilter
            PivotField field = pivot.ColumnFields[0];
            field.FilterByValue(0, PivotFilterType.ValueNotBetween, 300, 500);

            pivot.RefreshData();
            pivot.CalculateData();
            book.Save(Constants.destPath + "ValueNotBetween.xlsx");
            Assert.AreEqual("260", book.Worksheets[0].Cells["B18"].StringValue);
          
            book.Save(Constants.destPath + "ValueNotBetween.pdf");
        }
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


