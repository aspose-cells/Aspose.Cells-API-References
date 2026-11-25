---
title: "ValidationCollection.RemoveACell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ValidationCollection. Rimuove tutte le impostazioni di convalida sulla cella"
type: docs
url: /it/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Rimuove tutte le impostazioni di convalida sulla cella.

```csharp
public void RemoveACell(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice di riga della cella. |
| colonna | Int32 | L'indice di colonna della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi la convalida alla cella A1 (riga 0, colonna 0)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // Rimuovi la convalida dalla cella A1
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### Vedi anche

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


