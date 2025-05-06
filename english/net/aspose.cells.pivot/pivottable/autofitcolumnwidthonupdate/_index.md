---
title: PivotTable.AutofitColumnWidthOnUpdate
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether autofitting column width on update
type: docs
url: /net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Indicates whether autofitting column width on update

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Examples

```csharp
// Called: pt.AutofitColumnWidthOnUpdate = false;
[Test]
        public void Property_AutofitColumnWidthOnUpdate()
        {
            Aspose.Cells.Workbook wb = new Aspose.Cells.Workbook(Constants.PivotTableSourcePath + &quot;CELLSJAVA45323.xlsx&quot;);
            Worksheet worksheet = wb.Worksheets[&quot;PIVOT&quot;];
            PivotTable pt = worksheet.PivotTables[0];
            pt.AutofitColumnWidthOnUpdate = false;
            worksheet.RefreshPivotTables();
            wb.Save(Constants.PivotTableDestPath + &quot;CELLSJAVA45323.xlsx&quot;);
            wb = new Workbook(Constants.PivotTableDestPath + &quot;CELLSJAVA45323.xlsx&quot;);
            worksheet = wb.Worksheets[&quot;PIVOT&quot;];
            pt = worksheet.PivotTables[0];
            Assert.IsFalse(pt.AutofitColumnWidthOnUpdate );
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


