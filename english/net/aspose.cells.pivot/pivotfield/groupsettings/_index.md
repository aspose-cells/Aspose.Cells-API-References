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
// Called: Assert.IsTrue(pt.BaseFields[0].GroupSettings == null);
[Test]
        public void Property_GroupSettings()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CellsJava45720.xlsb");
            RefreshPivotTableCustomer(workbook, "PivotTable1", "Pivot Entry");
            //workbook.Worksheets.RefreshPivotTables();
            PivotTable pt = workbook.Worksheets["Pivot Entry"].PivotTables["PivotTable1"];
            Assert.AreEqual(80,pt.BaseFields.Count);
            Assert.IsTrue(pt.BaseFields[0].GroupSettings == null);
            workbook.Save(Constants.PivotTableDestPath + "CellsJava45720.xlsb");
        }
```

### See Also

* class [PivotFieldGroupSettings](../../pivotfieldgroupsettings/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


