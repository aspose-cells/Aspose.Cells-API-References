---
title: "Cells.UnMerge"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Annulla l'unione di un intervallo specificato di celle unite"
type: docs
url: /it/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Separa un intervallo specificato di celle unite.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstRow | Int32 | Prima riga di questo intervallo (indice zero) |
| firstColumn | Int32 | Prima colonna di questo intervallo (indice zero) |
| totalRows | Int32 | Numero di righe (indice a base 1) |
| totalColumns | Int32 | Numero di colonne (indice a base 1) |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Unisci prima le celle
            cells.Merge(0, 0, 2, 2);
            
            // Annulla l'unione delle celle precedentemente unite
            cells.UnMerge(0, 0, 2, 2);
            
            // Salva la cartella di lavoro
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


