---
title: "Cells.HideRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Versteckt eine Zeile"
type: docs
url: /de/net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Blendet eine Zeile aus.

```csharp
public void HideRow(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zeile 5 ausblenden
            worksheet.Cells.HideRow(5);
            
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


