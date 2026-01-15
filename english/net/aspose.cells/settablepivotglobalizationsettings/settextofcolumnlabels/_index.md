---
title: SettablePivotGlobalizationSettings.SetTextOfColumnLabels
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Column Labels label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

Gets the text of "Column Labels" label in the PivotTable.

```csharp
public void SetTextOfColumnLabels(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of column labels |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook (just for context)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Create an instance of SettablePivotGlobalizationSettings
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // Set custom text for the "Column Labels" label
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // Retrieve the current text to verify the change
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // Save the workbook (no pivot table is required for this demo)
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


