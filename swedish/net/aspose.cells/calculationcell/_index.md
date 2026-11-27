---
title: "Klass CalculationCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CalculationCell-klass. Representerar den beräkningsrelevanta data om en cell som beräknas"
type: docs
url: /sv/net/aspose.cells/calculationcell/
---
## CalculationCell class

Representerar den beräkningsrelevanta datan om en cell som beräknas.

```csharp
public class CalculationCell
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Hämtar Cell-objektet som beräknas. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Hämtar kolumnindex för cellen. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Hämtar radindex för cellen. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Hämtar Workbook-objektet. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Hämtar Worksheet-objektet där cellen finns. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Anger det beräknade värdet för cellen. |

### Anmärkningar

Användaren bör inte ändra någon data i Workbook under formelberäkningsprocessen, annars kan oväntade resultat eller undantag uppstå. Så är alla objekt som tillhandahålls av denna klass (såsom Cell-objektet av [`Cell`](./cell/)) endast för \"läsning\".

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
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

                // Visa grundläggande egenskaper
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Spara arbetsboken
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


