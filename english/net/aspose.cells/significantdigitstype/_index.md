---
title: Enum SignificantDigitsType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.SignificantDigitsType enum. Represents the type of significant digits for outputting numeric values
type: docs
url: /net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Represents the type of significant digits for outputting numeric values.

```csharp
public enum SignificantDigitsType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Digits15 | `0` | 15-digits |
| G17 | `1` | 17-digits by formatting the value with "G17". |
| Rounding17 | `2` | 17-digits by rounding the value. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook for demonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrate using each SignificantDigitsType enum value
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Set the significant digits type for the workbook
                    workbook.Settings.SignificantDigitsType = type;

                    // Display the current setting
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Add a sample value to demonstrate the setting
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Save the workbook with the current setting
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


