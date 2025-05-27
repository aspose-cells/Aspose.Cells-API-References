---
title: UnionRange.Name
second_title: Aspose.Cells for .NET API Reference
description: UnionRange property. Gets or sets the name of the range
type: docs
url: /net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Gets or sets the name of the range.

```csharp
public string Name { get; set; }
```

### Remarks

Named range is supported. For example,

range.Name = "Sheet1!MyRange";

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Create a range (changed from CreateUnionRange to CreateRange)
            Aspose.Cells.Range priceRange = worksheet.Cells.CreateRange("B2:B3");

            // Display current name (should be empty initially)
            Console.WriteLine("Current Name value: " + (priceRange.Name ?? "[null]"));

            // Set a name for the range
            priceRange.Name = "ProductPrices";

            // Demonstrate usage of the named range
            worksheet.Cells["D1"].PutValue("Total Price:");
            worksheet.Cells["E1"].Formula = "=SUM(ProductPrices)";

            // Calculate formulas
            workbook.CalculateFormula();

            // Display the effect of naming the range
            Console.WriteLine("Total price calculated using named range: " + worksheet.Cells["E1"].Value);

            // Save the workbook
            workbook.Save("UnionRangePropertyNameDemo.xlsx");
        }
    }
}
```

### See Also

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


