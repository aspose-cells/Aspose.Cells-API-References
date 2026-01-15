---
title: SettablePivotGlobalizationSettings.GetTextOfColumnLabels
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Column Labels label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfColumnLabels method

Gets the text of "Column Labels" label in the PivotTable.

```csharp
public override string GetTextOfColumnLabels()
```

### Return Value

The text of column labels

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for context
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Get the default text of column labels
                string columnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Default text of Column Labels: {columnLabelsText}");

                // Set custom text for column labels
                settings.SetTextOfColumnLabels("Custom Column Headers");

                // Get the updated text of column labels
                string updatedColumnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Updated text of Column Labels: {updatedColumnLabelsText}");

                // Save the workbook
                workbook.Save("GetTextOfColumnLabelsDemo.xlsx");
                Console.WriteLine("GetTextOfColumnLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


