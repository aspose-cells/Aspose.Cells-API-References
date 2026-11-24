---
title: "Cells.UnhideRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Blendet eine Zeile ein"
type: docs
url: /de/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Blendet eine Zeile ein.

```csharp
public void UnhideRow(int row, double height)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| Höhe | Double | Zeilenhöhe. Die Höhe der Zeile wird nur geändert, wenn die Zeile ausgeblendet ist und der angegebene Höhenwert positiv ist. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zeile 5 ausblenden
            worksheet.Cells.HideRow(5);
            
            // Zeile 5 mit einer Höhe von 12,75 einblenden
            worksheet.Cells.UnhideRow(5, 12.75);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


