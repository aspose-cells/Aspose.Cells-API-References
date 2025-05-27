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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Create conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Set condition range
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Add condition and set type
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "25");
            FormatCondition fc = fcc[conditionIndex];
            
            // Demonstrate Type property usage
            Console.WriteLine("Condition Type: " + fc.Type);
            
            // Save the workbook
            workbook.Save("ConditionalFormattingValuePropertyTypeDemo_out.xlsx");
        }
    }
}
```

### See Also

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


