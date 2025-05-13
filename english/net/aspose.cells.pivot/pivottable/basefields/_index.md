---
title: PivotTable.BaseFields
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns all base pivot fields in the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/basefields/
---
## PivotTable.BaseFields property

Returns all base pivot fields in the PivotTable.

```csharp
public PivotFieldCollection BaseFields { get; }
```

### Examples

```csharp
// Called: PivotFieldCollection fields = wb.Worksheets[0].PivotTables[0].BaseFields;
public void PivotTable_Property_BaseFields()
{
    Workbook wb = new Workbook(Constants.openPivottablePath + "AsposeItemsCache.xlsx");
    PivotFieldCollection fields = wb.Worksheets[0].PivotTables[0].BaseFields;
    for (int i = 0; i < fields.Count; i++)
    {
        PivotField field = fields[i];
        string[] t = field.OriginalItems;
        for (int j = 0; j < t.Length; j++)
            Console.WriteLine(t[j]);
    }
    //wb.Save("D:\\tttt.xlsx");
}
```

### See Also

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


