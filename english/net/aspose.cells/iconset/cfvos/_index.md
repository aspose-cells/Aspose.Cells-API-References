---
title: IconSet.Cfvos
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get the CFValueObjects instance
type: docs
url: /net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Get the CFValueObjects instance.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // Add conditional formatting
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Set range for conditional formatting
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // Add icon set condition
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // Set icon set type
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Access the Cfvos property (read-only)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Display information about the Cfvos collection
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Iterate through the collection and display each value
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Save the workbook
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


