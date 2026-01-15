---
title: SettablePivotGlobalizationSettings.SetTextOfEmptyData
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of blank label in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofemptydata/
---
## SettablePivotGlobalizationSettings.SetTextOfEmptyData method

Sets the text of "(blank)" label in the PivotTable.

```csharp
public void SetTextOfEmptyData(string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of empty data |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfEmptyDataWithStringDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data (optional, just for context)
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
                // Set custom text for empty data cells in a PivotTable
                settings.SetTextOfEmptyData("(no data)");

                // Verify the change
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Custom text for empty data: {emptyDataText}");

                // (Optional) Save the workbook – even though we didn't create a PivotTable,
                // this shows that the workbook can still be saved after the settings manipulation.
                workbook.Save("SetTextOfEmptyDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


