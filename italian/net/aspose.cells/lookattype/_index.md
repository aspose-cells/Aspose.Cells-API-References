---
title: "Enum LookAtType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.LookAtType enum. Rappresenta il tipo di ricerca"
type: docs
url: /it/net/aspose.cells/lookattype/
---
## LookAtType enumeration

Rappresenta il tipo di look-at.

```csharp
public enum LookAtType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Contains | `0` | Il valore della cella contiene l'oggetto da cercare. |
| StartWith | `1` | Il valore della cella inizia con l'oggetto da cercare. |
| EndWith | `2` | Il valore della cella termina con l'oggetto da cercare. |
| EntireContent | `3` | Il valore della cella è uguale all'oggetto da cercare. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // Istanzia l'oggetto cartella di lavoro
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Ottieni la raccolta Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Istanzia l'oggetto FindOptions
            FindOptions findOptions = new FindOptions();

            // Crea un'area Cells
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // Imposta l'area delle celle per le opzioni di ricerca
            findOptions.SetRange(ca);

            // Imposta le proprietà di ricerca
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Imposta LookAtType su Contains
            findOptions.LookAtType = LookAtType.Contains;

            // Trova la cella con un valore specifico
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


