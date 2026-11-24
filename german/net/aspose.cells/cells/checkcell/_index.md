---
title: "Cells.CheckCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt das Cell-Element oder null am angegebenen Zeilen- und Spaltenindex zurück"
type: docs
url: /de/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

Liefert das [`Cell`](../../cell/) Element oder null bei dem angegebenen Zeilen- und Spaltenindex der Zelle.

```csharp
public Cell CheckCell(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |
| column | Int32 | Spaltenindex |

### Rückgabewert

Gibt das Cell-Objekt zurück, wenn ein Cell-Objekt existiert. Gibt null zurück, wenn die Zelle nicht existiert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Werte in Cells setzen
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // Zellen mit der CheckCell-Methode und Int32-Parametern prüfen
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // Nicht vorhandene Zelle prüfen (liefert null zurück)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


