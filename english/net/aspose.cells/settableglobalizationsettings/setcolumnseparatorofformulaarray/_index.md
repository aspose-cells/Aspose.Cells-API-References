---
title: SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray
second_title: Aspose.Cells for .NET API Reference
description: SettableGlobalizationSettings method. Sets the separator for the items in arrays row data in formula
type: docs
url: /net/aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray method

Sets the separator for the items in array's row data in formula.

```csharp
public void SetColumnSeparatorOfFormulaArray(char c)
```

| Parameter | Type | Description |
| --- | --- | --- |
| c | Char | the specified separator |

### Examples

```csharp
namespace AsposeCellsExamples.SettableGlobalizationSettingsMethodSetColumnSeparatorOfFormulaArrayWithCharDemo
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetColumnSeparatorOfFormulaArrayWithCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            
            try
            {
                globalizationSettings.SetColumnSeparatorOfFormulaArray('|');
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                worksheet.Cells["A1"].SetArrayFormula("{1|2|3}", 1, 3);
                Console.WriteLine("Column separator for formula arrays set to '|'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetColumnSeparatorOfFormulaArray: {ex.Message}");
            }

            workbook.Save("SetColumnSeparatorOfFormulaArrayWithCharDemo.xlsx");
        }
    }
}
```

### See Also

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


