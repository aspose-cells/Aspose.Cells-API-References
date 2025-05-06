---
title: PivotFilter.MeasureFldIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotFilter property. Gets the measure field index of the pivot filter
type: docs
url: /net/aspose.cells.pivot/pivotfilter/measurefldindex/
---
## PivotFilter.MeasureFldIndex property

Gets the measure field index of the pivot filter.

```csharp
[Obsolete("Use PivotFilter.ValueFieldIndex property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int MeasureFldIndex { get; set; }
```

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: filter.MeasureFldIndex = 1;
public static void Property_MeasureFldIndex()
        {
            // Create a new workbook
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
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

            // Add a pivot table to the worksheet
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add(&quot;=Sheet1!A1:C9&quot;, &quot;A12&quot;, &quot;TestPivotTable&quot;);
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, &quot;fruit&quot;);
            pivot.AddFieldToArea(PivotFieldType.Column, &quot;year&quot;);
            pivot.AddFieldToArea(PivotFieldType.Data, &quot;amount&quot;);

            // Set pivot table style
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Add a pivot filter
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Set additional properties for the pivot filter
            filter.Value1 = &quot;SampleValue1&quot;;
            filter.Value2 = &quot;SampleValue2&quot;;
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = &quot;SampleFilter&quot;;
            filter.EvaluationOrder = 1;

            // Refresh and calculate the pivot table data
            pivot.RefreshData();
            pivot.CalculateData();

            // Save the workbook
            book.Save(&quot;PivotFilterExample.xlsx&quot;);
        }
```

### See Also

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


