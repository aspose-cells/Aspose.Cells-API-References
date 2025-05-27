---
title: Cell.StringValueWithoutFormat
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets cells value as string without any format
type: docs
url: /net/aspose.cells/cell/stringvaluewithoutformat/
---
## Cell.StringValueWithoutFormat property

Gets cell's value as string without any format.

```csharp
[Obsolete("Use GetStringValue(CellValueFormatStrategy) with CellValueFormatStrategy.None instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValueWithoutFormat { get; }
```

### Remarks

NOTE: This method is now obsolete. Instead, User should get the value object and format it according to the value type and the specific requirement. This property will be removed 12 months later since December 2020. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyStringValueWithoutFormatDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Access cell A1 and set numeric value with formatting
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(12345.6789);
            Style style = workbook.CreateStyle();
            style.Number = 4; // Currency format with 2 decimal places
            cell.SetStyle(style);

            // Demonstrate StringValue vs StringValueWithoutFormat
            Console.WriteLine("Formatted value (StringValue): " + cell.StringValue);
            Console.WriteLine("Raw value (StringValueWithoutFormat): " + cell.StringValueWithoutFormat);

            // Modify cell to contain date value with formatting
            cell.PutValue(DateTime.Now);
            Style dateStyle = workbook.CreateStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            cell.SetStyle(dateStyle);

            // Show values after format change
            Console.WriteLine("\nAfter date format update:");
            Console.WriteLine("Formatted date (StringValue): " + cell.StringValue);
            Console.WriteLine("Raw date value (StringValueWithoutFormat): " + cell.StringValueWithoutFormat);

            // Save the workbook
            workbook.Save("StringValueWithoutFormatDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


