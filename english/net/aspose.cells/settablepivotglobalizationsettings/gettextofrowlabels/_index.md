---
title: SettablePivotGlobalizationSettings.GetTextOfRowLabels
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Row Labels label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofrowlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfRowLabels method

Gets the text of "Row Labels" label in the PivotTable.

```csharp
public override string GetTextOfRowLabels()
```

### Return Value

The text of row labels

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data for context
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Set custom text for row labels
                settings.SetTextOfRowLabels("Custom Row Labels");

                // Get the text of row labels
                string rowLabelsText = settings.GetTextOfRowLabels();

                Console.WriteLine($"Text of Row Labels: {rowLabelsText}");

                // Save the workbook
                workbook.Save("GetTextOfRowLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


