---
title: "Cells.UngroupColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gruppierung von Spalten aufheben"
type: docs
url: /de/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Löst die Gruppierung von Spalten auf.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | Int32 | Der erste Spaltenindex, der aufgehoben werden soll. |
| lastIndex | Int32 | Der letzte Spaltenindex, der aufgehoben werden soll. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Spalten zuerst gruppieren, um das Aufheben der Gruppierung zu demonstrieren
            worksheet.Cells.GroupColumns(0, 2);

            // Spalten aufheben (0 bis 2)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


