---
title: PivotField.GroupSettings
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets the group settings of the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/groupsettings/
---
## PivotField.GroupSettings property

Gets the group settings of the pivot field.

```csharp
public PivotFieldGroupSettings GroupSettings { get; }
```

### Remarks

If this field is not grouped, Null will be returned.

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].BaseFields[1].GroupSettings == null);
public void PivotField_Property_GroupSettings()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + @"example.xlsx");
    Cells cells = workbook.Worksheets[0].Cells;

    cells["B4"].PutValue("c");
    workbook.Worksheets.RefreshPivotTables();
    Assert.AreEqual("c", cells["G18"].StringValue);
    Assert.IsTrue(workbook.Worksheets[0].PivotTables[0].BaseFields[1].GroupSettings == null);

    workbook = new Workbook(Constants.PivotTableSourcePath + @"example.xlsx");
    cells = workbook.Worksheets[0].Cells;

    cells["E5"].PutValue("c");
    workbook.Worksheets.RefreshPivotTables();
    Assert.AreEqual("c", cells["K8"].StringValue);
    Assert.AreEqual("8-9", cells["G14"].StringValue);
    Assert.AreEqual(5, workbook.Worksheets[0].PivotTables[0].BaseFields.Count);

}
```

### See Also

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


