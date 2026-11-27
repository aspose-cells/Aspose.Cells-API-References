---
title: "Cell.GetFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Hämta formeln för den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/getformula/
---
## Cell.GetFormula method

Hämta formeln för denna cell.

```csharp
public string GetFormula(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isR1C1 | Boolean | Om formeln behöver formateras som R1C1. |
| isLocal | Boolean | Om formeln behöver formateras enligt lokala inställningar. |

### Returvärde

formeln för den här cellen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och formler
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.PutValue(10);
            
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.PutValue(20);
            
            Cell cellC1 = worksheet.Cells["C1"];
            cellC1.Formula = "=A1+B1";
            
            // Demonstrera GetFormula med olika parametrar
            Console.WriteLine("Standard formula: " + cellC1.GetFormula(false, false));
            Console.WriteLine("Local formula: " + cellC1.GetFormula(false, true));
            
            // Ändra formelstil till lokal och visa skillnad
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("de-DE");
            Console.WriteLine("Local formula after culture change: " + cellC1.GetFormula(false, true));
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


