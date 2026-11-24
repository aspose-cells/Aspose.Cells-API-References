---
title: "Cell.GetFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt die Formel dieser Zelle zurück"
type: docs
url: /de/net/aspose.cells/cell/getformula/
---
## Cell.GetFormula method

Liefert die Formel dieser Zelle.

```csharp
public string GetFormula(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Rückgabewert

die Formel dieser Zelle.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Formeln hinzufügen
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.PutValue(10);
            
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.PutValue(20);
            
            Cell cellC1 = worksheet.Cells["C1"];
            cellC1.Formula = "=A1+B1";
            
            // Demonstration von GetFormula mit verschiedenen Parametern
            Console.WriteLine("Standard formula: " + cellC1.GetFormula(false, false));
            Console.WriteLine("Local formula: " + cellC1.GetFormula(false, true));
            
            // Formelstil auf lokal ändern und Unterschied zeigen
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("de-DE");
            Console.WriteLine("Local formula after culture change: " + cellC1.GetFormula(false, true));
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


