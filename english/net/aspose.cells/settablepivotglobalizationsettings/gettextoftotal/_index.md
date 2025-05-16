---
title: SettablePivotGlobalizationSettings.GetTextOfTotal
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text of Total label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

```csharp
public override string GetTextOfTotal()
```

### Return Value

The text of "Total" label

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);

            // Create pivot table with multiple data fields
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create custom globalization settings
            var settings = new CustomPivotGlobalizationSettings();

            try
            {
                // Get default "Total" text
                string defaultTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Default 'Total' text: {defaultTotalText}");

                // Change the "Total" text
                settings.SetTextOfTotal("Custom Total");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("GetTextOfTotal method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOfTotal method: {ex.Message}");
            }

            // Save the result
            workbook.Save("MethodGetTextOfTotalDemo.xlsx");
        }
    }

    public class CustomPivotGlobalizationSettings : GlobalizationSettings
    {
        private string _totalText = "Total";

        public string GetTextOfTotal()
        {
            return _totalText;
        }

        public void SetTextOfTotal(string text)
        {
            _totalText = text;
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


