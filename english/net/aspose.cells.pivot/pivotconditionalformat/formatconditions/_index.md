---
title: PivotConditionalFormat.FormatConditions
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat property. Get conditions for the pivot table conditional format 
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/formatconditions/
---
## PivotConditionalFormat.FormatConditions property

Get conditions for the pivot table conditional format .

```csharp
public FormatConditionCollection FormatConditions { get; }
```

### Examples

```csharp
// Called: FormatConditionCollection fcs = pfc.FormatConditions;
[Test]
        public void Property_FormatConditions()
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
            wb.Save(Constants.savePivottablePath + "40082.xlsx");
        }
```

### See Also

* class [FormatConditionCollection](../../../aspose.cells/formatconditioncollection/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


