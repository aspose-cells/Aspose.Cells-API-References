---
title: "Cell.IsSharedFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se la formula della cella fa parte di una formula condivisa"
type: docs
url: /it/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Indica se la formula della cella è parte di una formula condivisa.

```csharp
public bool IsSharedFormula { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta la formula condivisa in un intervallo
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // Verifica se le celle contengono una formula condivisa
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


