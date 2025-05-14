---
title: PivotField.ShowInOutlineForm
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether layout this field in outline form on the Pivot Table view
type: docs
url: /net/aspose.cells.pivot/pivotfield/showinoutlineform/
---
## PivotField.ShowInOutlineForm property

Indicates whether layout this field in outline form on the Pivot Table view

```csharp
public bool ShowInOutlineForm { get; set; }
```

### Examples

```csharp
// Called: wb.Worksheets[2].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
public void PivotField_Property_ShowInOutlineForm()
{

    Workbook wb = new Workbook(Constants.openPivottablePath + "Source.xlsx");
    Style style = wb.CreateStyle();
    style.Custom = "dd/mmm";
    wb.Worksheets[2].PivotTables[0].Format(9, 0, style);
    wb.Worksheets[2].PivotTables[0].Format(10, 0, style);
    wb.Worksheets[2].PivotTables[0].Format(11, 0, style);
    wb.Worksheets[2].PivotTables[0].Format(12, 0, style);
    wb.Worksheets[2].PivotTables[0].RowFields[0].IsAutoSubtotals = false;
    wb.Worksheets[2].PivotTables[0].RowFields[0].ShowInOutlineForm = false;
    wb.Worksheets[2].PivotTables[0].RefreshData();
    wb.Worksheets[2].PivotTables[0].CalculateData();
    wb.Save(Constants.savePivottablePath + "example.xlsx");
}
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


