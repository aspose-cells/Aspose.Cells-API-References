---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die nullbasierte Gliederungsebene der Spalte zurück"
type: docs
url: /de/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Gibt die Gliederungsebene (nullbasiert) der Spalte zurück.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Der Spalten‑Index |

### Rückgabewert

Die Gliederungsebene der Spalte

### Hinweise

Wenn die Spalte nicht gruppiert ist, wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gruppiere Spalten (die ersten 3 Spalten), ohne sie zu verbergen
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // Erhalte die Gliederungsebene der ersten Spalte
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


