---
title: "Cell.Copy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Copia i dati da una cella di origine"
type: docs
url: /it/net/aspose.cells/cell/copy/
---
## Cell.Copy method

Copia i dati da una cella di origine.

```csharp
public void Copy(Cell cell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | Cell | Oggetto [`Cell`](../) di origine. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCopyWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Imposta valori e stili nella cella di origine
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // Crea cella di destinazione
            Cell destCell = cells["B1"];

            // Copia dalla sorgente alla destinazione
            destCell.Copy(sourceCell);

            // Verifica la copia
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


