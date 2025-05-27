---
title: ConditionalFormattingValueCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingValueCollection property. Get the CFValueObject element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

Get the CFValueObject element at the specified index.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValueCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add conditional formatting
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Add condition and set format
            int conditionIndex = fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            FormatCondition fc = fcc[conditionIndex];
            
            // Get the values (using Formula1 and Formula2 for cell value conditions)
            Console.WriteLine("First value: " + fc.Formula1);
            Console.WriteLine("Second value: " + fc.Formula2);
            
            // Modify values
            fc.Formula1 = "20";
            fc.Formula2 = "80";
            
            Console.WriteLine("Updated first value: " + fc.Formula1);
            Console.WriteLine("Updated second value: " + fc.Formula2);
        }
    }
}
```

### See Also

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


