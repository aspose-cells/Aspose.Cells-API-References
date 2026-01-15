---
title: SettablePivotGlobalizationSettings.SetTextOfSubTotal
second_title: Aspose.Cells for .NET API Reference
description: SettablePivotGlobalizationSettings method. Sets the text of PivotFieldSubtotalType type in the PivotTable
type: docs
url: /net/aspose.cells/settablepivotglobalizationsettings/settextofsubtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfSubTotal method

Sets the text of [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) type in the PivotTable.

```csharp
public void SetTextOfSubTotal(PivotFieldSubtotalType subTotalType, string text)
```

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | PivotFieldSubtotalType | The [`PivotFieldSubtotalType`](../../../aspose.cells.pivot/pivotfieldsubtotaltype/) |
| text | String | The text of given type |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfSubTotalWithPivotFieldSubtoStringDemo
    {
        public static void Run()
        {
            // Create a new workbook (just for demonstration purposes)
            Workbook workbook = new Workbook();

            // Instance of SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Set custom text for the Sum subtotal
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Sum, "Custom Sum Total");

                // Verify the change
                string sumText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal text after change: {sumText}");

                // Set custom text for the Average subtotal
                settings.SetTextOfSubTotal(PivotFieldSubtotalType.Average, "Custom Average Total");

                // Verify the change
                string avgText = settings.GetTextOfSubTotal(PivotFieldSubtotalType.Average);
                Console.WriteLine($"Average subtotal text after change: {avgText}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfSubTotal: {ex.Message}");
            }

            // Save the workbook (no pivot table modifications in this demo)
            workbook.Save("SetTextOfSubTotalDemo.xlsx");
        }
    }
}
```

### See Also

* enum [PivotFieldSubtotalType](../../../aspose.cells.pivot/pivotfieldsubtotaltype/)
* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


