---
title: "Cells.CheckCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Restituisce l'elemento Cell o null all'indice di riga e colonna della cella specificati"
type: docs
url: /it/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Restituisce l'elemento [`Cell`](../../cell/) o null all'indice di riga e colonna della cella specificati.

```csharp
public Cell CheckCell(int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | Int32 | Indice della riga |
| colonna | Int32 | Indice colonna |

### Valore di ritorno

Restituisce l'oggetto Cell se esiste. Restituisce null se la cella non esiste.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta valori nelle celle
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // Verifica le celle usando il metodo CheckCell con parametri Int32
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // Verifica una cella inesistente (restituirà null)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### Vedi anche

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


