---
title: GlobalizationSettings.GetAllName
second_title: Aspose.Cells for .NET API Reference
description: GlobalizationSettings method. Gets the name of the All label in the PivotTable
type: docs
url: /net/aspose.cells/globalizationsettings/getallname/
---
## GlobalizationSettings.GetAllName method

Gets the name of the "(All)" label in the PivotTable.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOfAll() method instead.")]
public virtual string GetAllName()
```

### Return Value

The name of "(All)" label

### Remarks

NOTE: This member is now obsolete. Instead, please use GlobalizationSettings.GetColumnLabelsOfPivotTable() method. This property will be removed 12 months later since December 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetAllNameDemo
    {
        public static void Run()
        {
            // Create a new workbook with custom globalization settings
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Access the custom settings instance
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            try
            {
                // Call GetAllName method and display result
                string allName = settings.GetAllName();
                Console.WriteLine($"Custom (All) label: {allName}");

                // Create sample pivot table to demonstrate localization effect
                Worksheet worksheet = workbook.Worksheets[0];
                CreateSampleData(worksheet);
                CreatePivotTable(worksheet);

                Console.WriteLine("Demo executed successfully. Check output file's pivot table labels.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Save the modified workbook
            workbook.Save("MethodGetAllNameDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Create sample data for pivot table
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bikes";
            worksheet.Cells["A3"].Value = "Cars";
            worksheet.Cells["A4"].Value = "Bikes";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["B4"].Value = 1500;
        }

        private static void CreatePivotTable(Worksheet worksheet)
        {
            // Create pivot table using sample data
            int pivotIndex = worksheet.PivotTables.Add(
                "PivotTable",
                "A1:B4",
                "E3"
            );
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configure pivot table structure
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields[0]); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields[1]); // Sales

            // Refresh table to apply localization settings
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetAllName()
        {
            // Custom implementation returns localized "All" label
            return "[Custom All Selection]";
        }
    }
}
```

### See Also

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


