---
title: "CalculationData.CellColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData property. Hämtar kolumnindex för cellen där funktionen är"
type: docs
url: /sv/net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Hämtar kolumnindexet för cellen där funktionen är.

```csharp
public int CellColumn { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellColumnDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till exempeldata med formler i olika kolumner
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["B1"].PutValue(20);
                worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

                // Skapa beräkningsalternativ med anpassad motor
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellColumnDemoEngine();

                // Beräkna formler
                workbook.CalculateFormula(options);

                // Visa det beräknade resultatet
                Console.WriteLine("Calculated value in C1: " + worksheet.Cells["C1"].Value);

                // Spara resultatet
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellColumnDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data != null)
            {
                // Åtkomst till den skrivskyddade CellColumn-egenskapen
                int columnIndex = data.CellColumn;
                Console.WriteLine($"Function is in column index: {columnIndex}");

                // Demonstrera användning av kolumninformationen
                if (data.FunctionName == "SUM")
                {
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
}
```

### Se även

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


