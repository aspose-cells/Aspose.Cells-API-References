---
title: IconFilter.IconSetType
second_title: Aspose.Cells for .NET API Reference
description: IconFilter property. Gets and sets which icon set is used for this filter criteria
type: docs
url: /net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Gets and sets which icon set is used for this filter criteria.

```csharp
public IconSetType IconSetType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Create auto filter
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Get the icon filter
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Display current IconSetType (default is None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // Set to 3 arrows icon set
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Apply conditional formatting to visualize the icons
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Change to traffic lights icon set
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Save the result
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### See Also

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


