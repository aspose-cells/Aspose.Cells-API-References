---
title: "Cell.FormulaLocal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Ottieni la formula formattata per la locale della cella"
type: docs
url: /it/net/aspose.cells/cell/formulalocal/
---
## Cell.FormulaLocal property

Restituisce la formula formattata per la lingua locale della cella.

```csharp
public string FormulaLocal { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyFormulaLocalDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta la locale predefinita su tedesco per la dimostrazione
            workbook.Settings.Region = CountryCode.Germany;
            
            // Accedi alla cella A1
            Cell cell = worksheet.Cells["A1"];
            
            // Imposta la formula in formato standard (inglese)
            cell.Formula = "=SUM(B1:C1)";
            
            // Visualizza le formule sia in formato standard che locale
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Imposta la formula in formato locale (tedesco)
            cell.FormulaLocal = "=SUMME(B1:C1)";
            
            // Visualizza nuovamente le formule per mostrare la differenza
            Console.WriteLine("\nAfter setting FormulaLocal:");
            Console.WriteLine("Standard Formula: " + cell.Formula);
            Console.WriteLine("Localized Formula: " + cell.FormulaLocal);
            
            // Dimostra GetFormula con la localizzazione
            Console.WriteLine("\nUsing GetFormula:");
            Console.WriteLine("English formula: " + cell.GetFormula(false, false));
            Console.WriteLine("Localized formula: " + cell.GetFormula(false, true));
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


