---
title: "CalculationData.Cell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData-egenskap. Hämtar Cell-objektet där funktionen finns"
type: docs
url: /sv/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Hämtar Cell-objektet där funktionen är.

```csharp
public Cell Cell { get; }
```

### Anmärkningar

När du beräknar en formel utan att sätta den i en cell, till exempel med [`CalculateFormula`](../../worksheet/calculateformula/), beräknas formeln precis som om den hade satts i cell A1, så både [`CellRow`](../cellrow/) och [`CellColumn`](../cellcolumn/) är 0. Däremot kan cell A1 i kalkylbladet ha saknat en instans. Så i en sådan situation kommer den här egenskapen att vara null.

### Exempel

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
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till data för att göra exemplet meningsfullt
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Skapa beräkningsalternativ med anpassad motor
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellDemoEngine();

                // Beräkna formler med alternativ
                workbook.CalculateFormula(options);

                // Visa resultatet
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Spara resultatet
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
                // Läs‑endast Cell‑egenskapen
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

### Se även

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


