---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die nullbasierte Gliederungsebene der Zeile zurück"
type: docs
url: /de/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

Gibt die Gliederungsebene (nullbasiert) der Zeile zurück.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowIndex | Int32 | Der Zeilenindex. |

### Rückgabewert

Die Gliederungsebene (nullbasiert) der Zeile.

### Hinweise

Wenn die Zeile nicht gruppiert ist, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Zeilen 0-3 gruppieren (Ebene 1)
            cells.GroupRows(0, 3, false);
            
            // Zeilen 0-1 gruppieren (Ebene 2)
            cells.GroupRows(0, 1, false);

            // Gliederungsebene für jede Zeile abrufen
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // Alle Zeilen entgruppieren
            cells.UngroupRows(0, 3);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


