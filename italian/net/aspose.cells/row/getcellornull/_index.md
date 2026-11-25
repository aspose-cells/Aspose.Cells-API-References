---
title: "Row.GetCellOrNull"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Row. Ottiene la cella o null nell'indice specifico"
type: docs
url: /it/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

Ottiene la cella o null nell'indice specifico.

```csharp
public Cell GetCellOrNull(int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | Int32 | L'indice di colonna |

### Valore di ritorno

Restituisce l'oggetto cella se la cella esiste. Oppure restituisce null se l'oggetto cella non esiste.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Aggiungi dati di esempio
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // Ottieni la prima riga
            Row row = ws.Cells.Rows[0];

            // Dimostra GetCellOrNull con parametro Int32
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


