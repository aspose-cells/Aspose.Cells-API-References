---
title: ConditionalFormattingValue.Type
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValue property. Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set Value to null
type: docs
url: /net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Get or set the type of this conditional formatting value object. Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Max will auto set "Value" to null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Add some sample data (required for conditional formatting to exist)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Create a conditional formatting collection and add an IconSet condition
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // Obtain a ConditionalFormattingValue instance from the IconSet collection
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Set the Type to Percent and assign a corresponding value
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Read and display the Type and Value
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Change the Type to Min – per documentation this will nullify Value
                cfv.Type = FormatConditionValueType.Min;

                // Read and display the Type and Value again
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Save the workbook (the conditional formatting is part of the sheet)
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
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

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


