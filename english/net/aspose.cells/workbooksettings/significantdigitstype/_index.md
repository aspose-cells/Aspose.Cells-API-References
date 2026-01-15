---
title: WorkbookSettings.SignificantDigitsType
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is SignificantDigitsType
type: docs
url: /net/aspose.cells/workbooksettings/significantdigitstype/
---
## WorkbookSettings.SignificantDigitsType property

Gets and sets the type of significant digits for outputing numeric values in this workbook. Default value is [`SignificantDigitsType`](../../cellshelper/significantdigitstype/).

```csharp
public SignificantDigitsType SignificantDigitsType { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // Display the current SignificantDigitsType value
            Console.WriteLine("Current SignificantDigitsType: " + settings.SignificantDigitsType);

            // Demonstrate setting different SignificantDigitsType values
            settings.SignificantDigitsType = SignificantDigitsType.Digits15;
            Console.WriteLine("After setting to Digits15: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.G17;
            Console.WriteLine("After setting to G17: " + settings.SignificantDigitsType);

            settings.SignificantDigitsType = SignificantDigitsType.Rounding17;
            Console.WriteLine("After setting to Rounding17: " + settings.SignificantDigitsType);

            // Add some numeric data to demonstrate the effect
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(123.4567890123456789);
            worksheet.Cells["A2"].PutValue(9876543210.123456789);

            // Save the workbook
            workbook.Save("SignificantDigitsTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with SignificantDigitsType settings.");
        }
    }
}
```

### See Also

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


