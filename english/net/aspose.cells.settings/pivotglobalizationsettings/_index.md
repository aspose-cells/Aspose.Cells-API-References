---
title: Class PivotGlobalizationSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Settings.PivotGlobalizationSettings class. Represents the globalization settings for pivot tables
type: docs
url: /net/aspose.cells.settings/pivotglobalizationsettings/
---
## PivotGlobalizationSettings class

Represents the globalization settings for pivot tables.

```csharp
public class PivotGlobalizationSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [PivotGlobalizationSettings](pivotglobalizationsettings/)() | The default constructor. |

## Methods

| Name | Description |
| --- | --- |
| virtual [GetNameOfDataField](../../aspose.cells.settings/pivotglobalizationsettings/getnameofdatafield/)(ConsolidationFunction, string) | Gets the display name of data pivot field. The default format is "Sum Of Field". |
| virtual [GetShortTextOf12Months](../../aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/)() | Gets all short formatted string of 12 months. |
| virtual [GetTextOf4Quaters](../../aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/)() | Gets the local text of 4 Quaters. |
| virtual [GetTextOfAll](../../aspose.cells.settings/pivotglobalizationsettings/gettextofall/)() | Gets the text of "(All)" label in the PivotTable. |
| virtual [GetTextOfAllPeriods](../../aspose.cells.settings/pivotglobalizationsettings/gettextofallperiods/)() | Gets the localized text of "All Periods". |
| virtual [GetTextOfColumnLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofcolumnlabels/)() | Gets the text of "Column Labels" label in the PivotTable. |
| virtual [GetTextOfDataFieldHeader](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdatafieldheader/)() | Gets the the text of the value area field header in the PivotTable. |
| virtual [GetTextOfDays](../../aspose.cells.settings/pivotglobalizationsettings/gettextofdays/)() | Gets the local text of "Days". |
| virtual [GetTextOfEmptyData](../../aspose.cells.settings/pivotglobalizationsettings/gettextofemptydata/)() | Gets the text of "(blank)" label in the PivotTable. |
| virtual [GetTextOfGrandTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofgrandtotal/)() | Gets the text of "Grand Total" label in the PivotTable. |
| virtual [GetTextOfHours](../../aspose.cells.settings/pivotglobalizationsettings/gettextofhours/)() | Gets the local text of "Hours". |
| virtual [GetTextOfMinutes](../../aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/)() | Gets the local text of "Minutes". |
| virtual [GetTextOfMonths](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/)() | Gets the local text of "Months". |
| virtual [GetTextOfMultipleItems](../../aspose.cells.settings/pivotglobalizationsettings/gettextofmultipleitems/)() | Gets the text of "(Multiple Items)" label in the PivotTable. |
| virtual [GetTextOfProtectedName](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/)(string) | Gets the text for specified protected name. |
| virtual [GetTextOfProtection](../../aspose.cells.settings/pivotglobalizationsettings/gettextofprotection/)() | (**Obsolete.**) Gets the protection name in the PivotTable. |
| virtual [GetTextOfQuarters](../../aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/)() | Get the local text of "Quarters". |
| virtual [GetTextOfRange](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrange/)() | Gets the local text of "Range" |
| virtual [GetTextOfRowLabels](../../aspose.cells.settings/pivotglobalizationsettings/gettextofrowlabels/)() | Gets the text of "Row Labels" label in the PivotTable. |
| virtual [GetTextOfSeconds](../../aspose.cells.settings/pivotglobalizationsettings/gettextofseconds/)() | Gets the local text of "Seconds" |
| virtual [GetTextOfSubTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextofsubtotal/)(PivotFieldSubtotalType) | Gets the text of [`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable. |
| virtual [GetTextOfTotal](../../aspose.cells.settings/pivotglobalizationsettings/gettextoftotal/)() | Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area. |
| virtual [GetTextOfYears](../../aspose.cells.settings/pivotglobalizationsettings/gettextofyears/)() | Gets the local text of "Years". |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGlobalizationSettingsDemo
    {
        public static void PivotGlobalizationSettingsExample()
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
    }
}
```

### See Also

* namespace [Aspose.Cells.Settings](../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../)


