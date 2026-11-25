---
title: "ValidationCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ValidationCollection. Ottiene l'elemento Validation all'indice specificato"
type: docs
url: /it/net/aspose.cells/validationcollection/item/
---
## ValidationCollection indexer

Ottiene l'elemento [`Validation`](../../validation/) all'indice specificato.

```csharp
public Validation this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi la convalida dei dati alle celle
            ValidationCollection validations = sheet.Validations;
            
            // Prima area di convalida
            Validation validation1 = validations[validations.Add()];
            validation1.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 3 });
            
            // Seconda area di convalida
            Validation validation2 = validations[validations.Add()];
            validation2.AddArea(new CellArea { StartRow = 6, StartColumn = 1, EndRow = 6, EndColumn = 3 });

            // Accedi alla convalida usando la proprietà Item
            Validation firstValidation = validations[0];
            Console.WriteLine($"First validation has {firstValidation.Areas.Length} area(s)");

            // Verifica le aree
            foreach (CellArea area in firstValidation.Areas)
            {
                Console.WriteLine($"Area: {area.StartRow},{area.StartColumn} to {area.EndRow},{area.EndColumn}");
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


