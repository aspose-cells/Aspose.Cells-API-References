---
title: "Cells.CheckRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt das Row-Element oder null am angegebenen Zeilenindex zurück"
type: docs
url: /de/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Gibt das [`Row`](../../row/)‑Element oder null am angegebenen Zeilenindex zurück.

```csharp
public Row CheckRow(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |

### Rückgabewert

Gibt das [`Row`](../../row/)‑Objekt zurück, wenn das Zeilenobjekt existiert, andernfalls wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckRowWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Einige Daten befüllen
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // Überprüfen, ob die Zeile existiert, und das Zeilenobjekt abrufen
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // Nicht vorhandene Zeile prüfen
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### Siehe auch

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


