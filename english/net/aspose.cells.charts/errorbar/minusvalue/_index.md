---
title: ErrorBar.MinusValue
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents negative error amount when error bar type is Custom
type: docs
url: /net/aspose.cells.charts/errorbar/minusvalue/
---
## ErrorBar.MinusValue property

Represents negative error amount when error bar type is Custom.

```csharp
public string MinusValue { get; set; }
```

### Examples

```csharp
// Called: errorbar.MinusValue = &amp;quot;=A3&amp;quot;;
[Test]
        public void Property_MinusValue()
        {
            Workbook workbook = new Workbook();
            workbook = TestColumn.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            ErrorBar errorbar = chart.NSeries[0].YErrorBar;
            errorbar.DisplayType = ErrorBarDisplayType.Both;
            errorbar.Type = ErrorBarType.Custom;
              errorbar.PlusValue = &quot;=A2&quot;;
              errorbar.MinusValue = &quot;=A3&quot;;

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


