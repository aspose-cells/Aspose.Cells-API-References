---
title: "CalculationCell.SetCalculatedValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationCell metod. Anger det beräknade värdet för cellen"
type: docs
url: /sv/net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Anger det beräknade värdet för cellen.

```csharp
public void SetCalculatedValue(object v)
```

### Anmärkningar

Användaren kan ange det beräknade resultatet med den här metoden för att ignorera den automatiska beräkningen för cellen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Skapa en CalculationCell-instans med reflektion eftersom konstruktorn är icke-publik
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Ange ett beräknat värde med SetCalculatedValue-metoden
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Visa information om cellen
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Spara arbetsboken
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


