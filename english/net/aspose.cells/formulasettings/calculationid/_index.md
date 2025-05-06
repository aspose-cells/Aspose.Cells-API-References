---
title: FormulaSettings.CalculationId
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Specifies the version of the calculation engine used to calculate values in the workbook
type: docs
url: /net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Specifies the version of the calculation engine used to calculate values in the workbook.

```csharp
public string CalculationId { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

### Examples

```csharp
// Called: wb.Settings.FormulaSettings.CalculationId = &amp;quot;999999&amp;quot;;
private Workbook Property_CalculationId()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            Util.SetHintMessage(cells[0, 1],
                &quot;Change the value of A1, A2:D2 should be re-calculated and kept same with A1 automatically, and A3:D3 should all be \&quot;OK\&quot;&quot;);
            cells[1, 0].Formula = &quot;=INDIRECT(\&quot;A1\&quot;)&quot;;
            cells[1, 1].SetSharedFormula(&quot;=INDIRECT(\&quot;A1\&quot;)&quot;, 1, 3);
            cells[1, 4].SetArrayFormula(&quot;=INDIRECT(\&quot;A1\&quot;)&quot;, 1, 3);
            cells[2, 0].SetSharedFormula(&quot;=IF(A2=$A$1,\&quot;OK\&quot;,\&quot;ERROR!\&quot;)&quot;, 1, 7);
            wb.CalculateFormula(false);
            wb.Settings.FormulaSettings.CalculationId = &quot;999999&quot;;
            wb.Settings.FormulaSettings.CalculateOnOpen = false;
            return wb;
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


