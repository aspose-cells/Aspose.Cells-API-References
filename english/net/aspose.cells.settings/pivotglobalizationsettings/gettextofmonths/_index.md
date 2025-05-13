---
title: PivotGlobalizationSettings.GetTextOfMonths
second_title: Aspose.Cells for .NET API Reference
description: PivotGlobalizationSettings method. Gets the local text of Months
type: docs
url: /net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

Gets the local text of "Months".

```csharp
public virtual string GetTextOfMonths()
```

### Examples

```csharp
// Called: Console.WriteLine("Text of Months: " + globalizationSettings.GetTextOfMonths());
public static void PivotGlobalizationSettings_Method_GetTextOfMonths()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Fruit");
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["B5"].PutValue(250);

            // Create a pivot table
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Create an instance of PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstrate the use of various methods
            Console.WriteLine("Text of Total: " + globalizationSettings.GetTextOfTotal());
            Console.WriteLine("Text of Grand Total: " + globalizationSettings.GetTextOfGrandTotal());
            Console.WriteLine("Text of Multiple Items: " + globalizationSettings.GetTextOfMultipleItems());
            Console.WriteLine("Text of All: " + globalizationSettings.GetTextOfAll());
            Console.WriteLine("Text of Protection: " + globalizationSettings.GetTextOfProtection());
            Console.WriteLine("Text of Column Labels: " + globalizationSettings.GetTextOfColumnLabels());
            Console.WriteLine("Text of Row Labels: " + globalizationSettings.GetTextOfRowLabels());
            Console.WriteLine("Text of Empty Data: " + globalizationSettings.GetTextOfEmptyData());
            Console.WriteLine("Text of Data Field Header: " + globalizationSettings.GetTextOfDataFieldHeader());
            Console.WriteLine("Text of Years: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Text of Quarters: " + globalizationSettings.GetTextOfQuarters());
            Console.WriteLine("Text of Months: " + globalizationSettings.GetTextOfMonths());
            Console.WriteLine("Text of Days: " + globalizationSettings.GetTextOfDays());
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
            Console.WriteLine("Text of Range: " + globalizationSettings.GetTextOfRange());

            // Example of GetTextOfProtectedName method
            string protectedName = "ProtectedNameExample";
            Console.WriteLine("Text of Protected Name: " + globalizationSettings.GetTextOfProtectedName(protectedName));

            // Example of GetTextOfSubTotal method
            PivotFieldSubtotalType subTotalType = PivotFieldSubtotalType.Sum;
            Console.WriteLine("Text of SubTotal (Sum): " + globalizationSettings.GetTextOfSubTotal(subTotalType));

            // Save the workbook
            workbook.Save("PivotGlobalizationSettingsExample.xlsx");
        }
```

### See Also

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


