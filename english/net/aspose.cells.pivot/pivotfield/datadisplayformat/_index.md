---
title: PivotField.DataDisplayFormat
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents how to display the values in a data field of the pivot report
type: docs
url: /net/aspose.cells.pivot/pivotfield/datadisplayformat/
---
## PivotField.DataDisplayFormat property

Represents how to display the values in a data field of the pivot report.

```csharp
[Obsolete("Use PivotField.ShowValuesSetting.CalculationType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldDataDisplayFormat DataDisplayFormat { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotField.ShowValuesSetting.CalculationType property instead. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: dataField.DataDisplayFormat = PivotFieldDataDisplayFormat.PercentageOfTotal;
public static void Property_DataDisplayFormat()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Add some sample data
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
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add(&quot;=Sheet1!A1:C9&quot;, &quot;A12&quot;, &quot;TestPivotTable&quot;);
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, &quot;fruit&quot;);
            pivot.AddFieldToArea(PivotFieldType.Column, &quot;year&quot;);
            pivot.AddFieldToArea(PivotFieldType.Data, &quot;amount&quot;);

            // Set the pivot table style
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Change PivotField&apos;s attributes
            PivotField dataField = pivot.DataFields[0];
            dataField.DisplayName = &quot;custom display name&quot;;

            // Set DataDisplayFormat
            dataField.DataDisplayFormat = PivotFieldDataDisplayFormat.PercentageOfTotal;

            // Refresh and calculate data
            pivot.RefreshData();
            pivot.CalculateData();

            // Save the workbook
            workbook.Save(&quot;PivotFieldDataDisplayFormatExample.xlsx&quot;);
        }
```

### See Also

* enum [PivotFieldDataDisplayFormat](../../pivotfielddatadisplayformat/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


