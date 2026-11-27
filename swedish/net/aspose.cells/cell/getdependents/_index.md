---
title: "Cell.GetDependents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämta alla celler vars formel refererar direkt till den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Hämta alla celler vars formel refererar direkt till denna cell.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isAll | Boolean | Anger om formler i andra arbetsblad ska kontrolleras |

### Anmärkningar

Om en referens som innehåller den här cellen förekommer i en cells formel, kommer den cellen att betraktas som beroende av den här cellen, oavsett om referensen eller den här cellen används vid beräkning. Till exempel, även om cell A2 i formeln "=IF(TRUE,A1,A2)" inte används vid beräkning, tas denna formel fortfarande som A2:s beroende. För att få de formler vars beräknade resultat beror på den här cellen, använd [`GetDependentsInCalculation`](../getdependentsincalculation/). När beroenden spåras för en cell analyseras och kontrolleras alla formler i arbetsboken eller arbetsbladet. Det är alltså en tidskrävande process. Om användaren behöver spåra beroenden för många celler kan användning av denna metod leda till dålig prestanda. Av prestandaskäl bör användaren istället använda [`GetDependentsInCalculation`](../getdependentsincalculation/). Eller så kan användaren först samla ett föregångarmapp för alla celler med [`GetPrecedents`](../getprecedents/), och sedan bygga ett beroendemapp baserat på föregångarmappen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ställ in formler som refererar till B1
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // Beräkna formler
            workbook.CalculateFormula();

            // Hämta alla celler som beror på B1 (rekursivt)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


