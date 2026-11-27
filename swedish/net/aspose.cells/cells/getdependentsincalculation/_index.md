---
title: "Cells.GetDependentsInCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar alla celler vars beräknade resultat beror på en specifik cell"
type: docs
url: /sv/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Hämtar alla celler vars beräknade resultat beror på en specifik cell.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för den specifika cellen |
| column | Int32 | Kolumnindex för den specifika cellen. |
| rekursiv | Boolean | Anger om de returnerar de beroenden som inte refererar direkt till den specifika cellen utan refererar till andra löv för den cellen. |

### Returvärde

Enumerator för att enumerera alla beroende (Cell-objekt)

### Anmärkningar

För att använda denna metod, se till att arbetsboken har satts till true för [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) och har beräknats fullt ut med denna inställning. Om det inte finns någon formelreferens till denna cell, returneras null. För mer detaljer och exempel, se [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/)

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och beräkna formler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in formelberoenden:
            // C1 = 10 (källvärde)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // Beräkna formler för att etablera beroenden
            workbook.CalculateFormula();

            try
            {
                // Hämta beroenden för cell C1 (rad 0, kolumn 2) med rekursiv kontroll
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


