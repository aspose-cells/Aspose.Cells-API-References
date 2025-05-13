---
title: PivotFieldCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection property. Gets the count of the pivotFields
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/count/
---
## PivotFieldCollection.Count property

Gets the count of the pivotFields.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(80,pt.BaseFields.Count);
public void PivotFieldCollection_Property_Count()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsb");
    RefreshPivotTableCustomer(workbook, "PivotTable1", "Pivot Entry");
    //workbook.Worksheets.RefreshPivotTables();
    PivotTable pt = workbook.Worksheets["Pivot Entry"].PivotTables["PivotTable1"];
    Assert.AreEqual(80,pt.BaseFields.Count);
    Assert.IsTrue(pt.BaseFields[0].GroupSettings == null);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsb");
}
```

### See Also

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


