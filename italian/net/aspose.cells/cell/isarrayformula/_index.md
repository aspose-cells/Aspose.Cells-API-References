---
title: "Cell.IsArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se la formula della cella è una formula di matrice"
type: docs
url: /it/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Indica se la formula della cella è una formula array.

```csharp
public bool IsArrayFormula { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una formula matriciale nella cella B2
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // Verifica se la cella contiene una formula matriciale
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // Restituisci il risultato
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // Salva la cartella di lavoro
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


