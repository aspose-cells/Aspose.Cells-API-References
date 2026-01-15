---
title: SettablePivotGlobalizationSettings.GetTextOfEmptyData
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of blank label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofemptydata/
---
## SettablePivotGlobalizationSettings.GetTextOfEmptyData method

Gets the text of "(blank)" label in the PivotTable.

```csharp
public override string GetTextOfEmptyData()
```

### Return Value

The text of empty data

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Get the default text for empty data
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Default text for empty data: '{emptyDataText}'");

                // Set a custom text for empty data
                settings.SetTextOfEmptyData("No Data Available");

                // Get the updated text for empty data
                string updatedEmptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Updated text for empty data: '{updatedEmptyDataText}'");

                // Apply settings to workbook
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
                globalizationSettings.PivotSettings = settings;
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Save the workbook
                workbook.Save("GetTextOfEmptyDataDemo.xlsx");
                Console.WriteLine("GetTextOfEmptyData method demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


