---
title: "Cells.GetCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Restituisce l'elemento Cell o null all'indice di riga e colonna della cella specificati"
type: docs
url: /it/net/aspose.cells/cells/getcell/
---
## Cells.GetCell method

Restituisce l'elemento [`Cell`](../../cell/) o null all'indice di riga e colonna della cella specificati.

```csharp
[Obsolete("Use Cells.CheckCell(int row, int column) instead.")]
public Cell GetCell(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |
| colonna | Int32 | Indice colonna |

### Valore di ritorno

Restituisce l'oggetto Cell se esiste. Restituisce null se la cella non esiste.

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo CheckCell(int row, int column). Questo metodo sarà rimosso 12 mesi dopo, a partire da febbraio 2024. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla cella alla riga 1, colonna 2 (indice basato su 0)
            Cell cell = worksheet.Cells.GetCell(1, 2);
            
            // Imposta valore e stile per la dimostrazione
            cell.PutValue("Test Value");
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("GetCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


