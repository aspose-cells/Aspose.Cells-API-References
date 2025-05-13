---
title: PivotTable.GetChildren
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the Children Pivot Tables which use this PivotTable data as data source
type: docs
url: /net/aspose.cells.pivot/pivottable/getchildren/
---
## PivotTable.GetChildren method

Gets the Children Pivot Tables which use this PivotTable data as data source.

```csharp
public PivotTable[] GetChildren()
```

### Return Value

the PivotTable array object

### Examples

```csharp
// Called: foreach (PivotTable childTable in table.GetChildren())
public void PivotTable_Method_GetChildren()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46645_";

    var path = filePath + @"BigReportWithUserDataAnonyme.xlsx";
    using (var workbook = new Workbook(path))
    {
        foreach (Worksheet worksheet in workbook.Worksheets)
        {
            foreach (PivotTable table in worksheet.PivotTables)
            {
                foreach (PivotTable childTable in table.GetChildren())
                {
                    //...
                }
            }
        }
    }
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


