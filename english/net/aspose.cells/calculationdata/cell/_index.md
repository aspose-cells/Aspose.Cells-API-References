---
title: CalculationData.Cell
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the Cell object where the function is
type: docs
url: /net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Gets the Cell object where the function is.

```csharp
public Cell Cell { get; }
```

### Remarks

When calculating a formula without setting it to a cell, such as by [`CalculateFormula`](../../worksheet/calculateformula/), the formula will be calculated just like it has been set to cell A1, so both [`CellRow`](../cellrow/) and [`CellColumn`](../cellcolumn/) are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Create a new workbook
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Add some data to make the example meaningful
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Create calculation options with custom engine
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellDemoEngine();

                // Calculate formulas with options
                workbook.CalculateFormula(options);

                // Display the result
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Save the result
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Access the read-only Cell property
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### See Also

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


