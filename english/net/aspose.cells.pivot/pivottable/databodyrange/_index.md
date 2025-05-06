---
title: PivotTable.DataBodyRange
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a CellArea object that represents the range that contains the data area in the list between the header row and the insert row. Readonly
type: docs
url: /net/aspose.cells.pivot/pivottable/databodyrange/
---
## PivotTable.DataBodyRange property

Returns a [`CellArea`](../../../aspose.cells/cellarea/) object that represents the range that contains the data area in the list between the header row and the insert row. Read-only.

```csharp
public CellArea DataBodyRange { get; }
```

### Examples

```csharp
// Called: fcc.AddArea(pivot.DataBodyRange);
public static void Property_DataBodyRange()
        {
            // Create a new Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate data
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

            // Create a PivotTable
            PivotTableCollection pivots = sheet.PivotTables;
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

            // Set properties of PivotFormatCondition
            pfc.ScopeType = PivotConditionFormatScopeType.Data;
            pfc.RuleType = PivotConditionFormatRuleType.All;

            // Refresh and calculate data
            pivot.RefreshData();
            pivot.CalculateData();

            // Save the workbook
            workbook.Save(&quot;PivotFormatConditionExample.xlsx&quot;);
        }
```

### See Also

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


