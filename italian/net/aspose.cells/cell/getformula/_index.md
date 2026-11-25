---
title: "Cell.GetFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Cell metodo. Ottieni la formula di questa cella"
type: docs
url: /it/net/aspose.cells/cell/getformula/
---
## Cell.GetFormula method

Ottieni la formula di questa cella.

```csharp
public string GetFormula(bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Valore di ritorno

la formula di questa cella.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e formule
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.PutValue(10);
            
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.PutValue(20);
            
            Cell cellC1 = worksheet.Cells["C1"];
            cellC1.Formula = "=A1+B1";
            
            // Dimostra GetFormula con parametri diversi
            Console.WriteLine("Standard formula: " + cellC1.GetFormula(false, false));
            Console.WriteLine("Local formula: " + cellC1.GetFormula(false, true));
            
            // Cambia lo stile della formula a locale e mostra la differenza
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("de-DE");
            Console.WriteLine("Local formula after culture change: " + cellC1.GetFormula(false, true));
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


