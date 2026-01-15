---
title: SettablePivotGlobalizationSettings.GetTextOfProtectedName
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Gets the text for specified protected name
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Gets the text for specified protected name.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |

### Return Value

The local prorected names of PivotTable.

### Remarks

In Ms Excel, some names are not allowed to be used as the name of PivotFields in PivotTable. They are different in different region, user may specify them explicitly according to the used region.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data for context
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Create an instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Set a custom text for a protected name
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Get the text of the protected name
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Save the workbook
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


