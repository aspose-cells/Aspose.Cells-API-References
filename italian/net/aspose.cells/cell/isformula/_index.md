---
title: "Cell.IsFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Indica se la cella specificata contiene una formula"
type: docs
url: /it/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Rappresenta se la cella specificata contiene una formula.

```csharp
public bool IsFormula { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi formula alla cella A1
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // Aggiungi valore semplice alla cella A2
            worksheet.Cells["A2"].PutValue("Test");
            
            // Verifica se le celle contengono formule
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


