---
title: "Validation.RemoveACell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di convalida. Rimuovi le impostazioni di convalida nella cella"
type: docs
url: /it/net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

Rimuovi le impostazioni di convalida nella cella.

```csharp
public void RemoveACell(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi la convalida dei dati alla prima cella
            Validation validation = worksheet.Validations[0];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.Type = ValidationType.List;
            validation.Formula1 = "1,2,3";
            
            // Aggiungi un'altra cella alla convalida
            validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
            
            // Rimuovi la seconda cella dalla convalida
            validation.RemoveACell(1, 1);
            
            Console.WriteLine("Cell removed from validation successfully.");
        }
    }
}
```

### Vedi anche

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


