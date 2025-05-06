---
title: PivotTable.PivotFormatConditions
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the Format Conditions of the pivot table
type: docs
url: /net/aspose.cells.pivot/pivottable/pivotformatconditions/
---
## PivotTable.PivotFormatConditions property

Gets the Format Conditions of the pivot table.

```csharp
[Obsolete("Use PivotTable.ConditionalFormats property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFormatConditionCollection PivotFormatConditions { get; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotTable.ConditionalFormats property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
public static void Property_PivotFormatConditions()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Add some data to the worksheet
            cells[0, 0].Value = &quot;fruit&quot;;
            cells[1, 0].Value = &quot;grape&quot;;
            cells[2, 0].Value = &quot;blueberry&quot;;
            cells[3, 0].Value = &quot;kiwi&quot;;
            cells[4, 0].Value = &quot;cherry&quot;;
            cells[5, 0].Value = &quot;grape&quot;;
            cells[6, 0].Value = &quot;blueberry&quot;;
            cells[7, 0].Value = &quot;kiwi&quot;;
            cells[8, 0].Value = &quot;cherry&quot;;

            cells[0, 1].Value = &quot;year&quot;;
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = &quot;amount&quot;;
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Add a pivot table
            PivotTableCollection pivots = worksheet.PivotTables;
            int pivotIndex = pivots.Add(&quot;=Sheet1!A1:C9&quot;, &quot;A12&quot;, &quot;TestPivotTable&quot;);
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, &quot;fruit&quot;);
            pivot.AddFieldToArea(PivotFieldType.Column, &quot;year&quot;);
            pivot.AddFieldToArea(PivotFieldType.Data, &quot;amount&quot;);

            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Add PivotFormatCondition
            int formatIndex = pivot.PivotFormatConditions.Add();
            PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            FormatConditionCollection fcc = pfc.FormatConditions;
            fcc.AddArea(pivot.DataBodyRange);
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = &quot;100&quot;;
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;

            // Set the scope type for the pivot table condition format
            pfc.ScopeType = PivotConditionFormatScopeType.Data;

            pivot.RefreshData();
            pivot.CalculateData();

            // Save the workbook
            workbook.Save(&quot;PivotConditionFormatScopeTypeExample.xlsx&quot;);
        }
```

### See Also

* class [PivotFormatConditionCollection](../../pivotformatconditioncollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


