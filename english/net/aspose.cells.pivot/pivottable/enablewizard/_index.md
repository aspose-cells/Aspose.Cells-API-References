---
title: PivotTable.EnableWizard
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Indicates whether the PivotTable Wizard is available
type: docs
url: /net/aspose.cells.pivot/pivottable/enablewizard/
---
## PivotTable.EnableWizard property

Indicates whether the PivotTable Wizard is available.

```csharp
public bool EnableWizard { get; set; }
```

### Examples

```csharp
// Called: pt.EnableWizard = false;
[Test]
        public void Property_EnableWizard()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA42680_&quot;;

            Workbook wb = new Workbook(filePath + &quot;pivot_table_test.xlsx&quot;);
            PivotTable pt = wb.Worksheets[0].PivotTables[0];
            pt.EnableWizard = false;
            wb.Save(CreateFolder(filePath) + &quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


