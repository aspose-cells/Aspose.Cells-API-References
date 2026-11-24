---
title: "Cell.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Kopiert Daten aus einer Quellzelle"
type: docs
url: /de/net/aspose.cells/cell/copy/
---
## Cell.Copy method

Kopiert Daten aus einer Quellzelle.

```csharp
public void Copy(Cell cell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | Cell | Quell-[`Cell`](../)-Objekt. |

### Beispiele

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

            // Setzen Sie Werte und Stile in der Quellzelle
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // Erstellen Sie die Zielzelle
            Cell destCell = cells["B1"];

            // Kopieren Sie von der Quelle zur Zielzelle
            destCell.Copy(sourceCell);

            // Überprüfen Sie die Kopie
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


