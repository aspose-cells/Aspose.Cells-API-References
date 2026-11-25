---
title: "ValidationCollection.GetValidationInCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ValidationCollection. Ottiene la convalida applicata alla cella specificata"
type: docs
url: /it/net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

Ottiene la convalida applicata alla cella specificata.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | L'indice della riga. |
| colonna | Int32 | L'indice della colonna. |

### Valore di ritorno

Restituisce un oggetto [`Validation`](../../validation/) o null se non esiste alcuna convalida per la cella specificata

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodGetValidationInCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi la convalida dei dati alla cella A1 (0,0)
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "\"Option1,Option2,Option3\"";
            
            // Crea CellArea con StartRow, StartColumn, EndRow, EndColumn
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Ottieni la convalida dalla cella A1 (0,0)
            Validation validationInCell = worksheet.Validations.GetValidationInCell(0, 0);
            
            if (validationInCell != null && validationInCell.Type == ValidationType.List)
            {
                Console.WriteLine("Cell A1 has list validation with formula: " + validationInCell.Formula1);
            }
        }
    }
}
```

### Vedi anche

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


