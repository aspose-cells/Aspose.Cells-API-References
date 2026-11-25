---
title: "Cell.IsDynamicArrayFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se la formula della cella è una formula di array dinamico (true) o una formula di array legacy (false)"
type: docs
url: /it/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Indica se la formula della cella è una formula array dinamica (true) o una formula array legacy (false).

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta una formula di array dinamico nella cella A1
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // Verifica se la cella contiene una formula di array dinamico
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // Salva la cartella di lavoro
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


