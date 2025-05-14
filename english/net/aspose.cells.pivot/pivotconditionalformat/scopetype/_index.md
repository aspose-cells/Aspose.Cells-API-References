---
title: PivotConditionalFormat.ScopeType
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat property. Get and set scope type for the pivot table conditional format 
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

Get and set scope type for the pivot table conditional format .

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### Examples

```csharp
// Called: pfc.ScopeType = PivotConditionFormatScopeType.Data;
public void PivotConditionalFormat_Property_ScopeType()
{
    Workbook wb = new Workbook(Constants.openPivottablePath + "aa.xlsx");

    int index = wb.Worksheets[0].PivotTables[0].ConditionalFormats.Add();
    PivotConditionalFormat pfc = wb.Worksheets[0].PivotTables[0].ConditionalFormats[index];
    pfc.ScopeType = PivotConditionFormatScopeType.Data;
    FormatConditionCollection fcs = pfc.FormatConditions;
    CellArea ca = new CellArea();
    ca.StartRow = 9;
    ca.EndRow = 9;
    ca.StartColumn = 5;
    ca.EndColumn = 5;
    int[] t = fcs.Add(ca, FormatConditionType.ColorScale, OperatorType.Equal, "", "");
    FormatCondition fc = fcs[t[0]];
    ColorScale scale = fc.ColorScale;
    scale.MidColor = Color.Red;
    scale.MinCfvo.Type = FormatConditionValueType.Max;
    scale.MinCfvo.Value = 10;
    wb.Save(Constants.savePivottablePath + "example.xlsx");
}
```

### See Also

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


