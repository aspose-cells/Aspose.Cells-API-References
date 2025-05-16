---
title: SettablePivotGlobalizationSettings.SetTextOfProtectedName
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text for specific protected name
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofprotectedname/
---
## SettablePivotGlobalizationSettings.SetTextOfProtectedName method

Sets the text for specific protected name.

```csharp
public void SetTextOfProtectedName(string protectedName, string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |
| text | String | The local prorected names of PivotTable. |

### Examples

```csharp
namespace AsposeCellsExamples.SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameWithStringStringDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameWithStringStringDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Category";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "Fruits";
            worksheet.Cells["C2"].Value = 1500;
            worksheet.Cells["A3"].Value = "Carrot";
            worksheet.Cells["B3"].Value = "Vegetables";
            worksheet.Cells["C3"].Value = 2000;

            // Create pivot table
            var pivotIndex = worksheet.PivotTables.Add("A1:C3", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Create globalization settings
            var settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Call SetTextOfProtectedName method to change protected name text
                settings.SetTextOfProtectedName("ProtectedName1", "Custom Protected Text");

                // Apply settings to workbook
                workbook.Settings.GlobalizationSettings = settings as GlobalizationSettings;

                // Refresh pivot table to apply changes
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("SetTextOfProtectedName method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfProtectedName method: {ex.Message}");
            }

            // Save the result
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameDemo.xlsx");
        }
    }

    public class SettablePivotGlobalizationSettings : GlobalizationSettings
    {
        public void SetTextOfProtectedName(string protectedName, string text)
        {
            // Implementation would store the custom text for the protected name
        }

        public string GetTextOfProtectedName(string protectedName)
        {
            return null; // Implementation would return the custom text if set
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


