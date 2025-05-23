---
title: ErrorBar.PlusValue
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents positive error amount when error bar type is Custom
type: docs
url: /net/aspose.cells.charts/errorbar/plusvalue/
---
## ErrorBar.PlusValue property

Represents positive error amount when error bar type is Custom.

```csharp
public string PlusValue { get; set; }
```

### Examples

```csharp
// Called: errorbar.PlusValue = "=A2";
public void ErrorBar_Property_PlusValue()
{
    Workbook workbook = new Workbook();
    workbook = TestColumn.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    ErrorBar errorbar = chart.NSeries[0].YErrorBar;
    errorbar.DisplayType = ErrorBarDisplayType.Both;
    errorbar.Type = ErrorBarType.Custom;
      errorbar.PlusValue = "=A2";
      errorbar.MinusValue = "=A3";

    checkErrorBarType_Custom(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkErrorBarType_Custom(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkErrorBarType_Custom(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


