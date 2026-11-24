---
title: "Cells.ApplyStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells‑Methode. Wendet Formate für ein gesamtes Arbeitsblatt an"
type: docs
url: /de/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Wendet Formate für ein ganzes Arbeitsblatt an.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Das Stil‑Objekt, das angewendet wird. |
| Flag | StyleFlag | Flags, die die angewendeten Formatierungseigenschaften angeben. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            
            // Erstelle einen Stil und setze den Textumbruch
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // Erstelle Stil-Flagge und aktiviere die Textumbruch-Flagge
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Wende den Stil auf alle Zellen im Arbeitsblatt an
            sheet.Cells.ApplyStyle(style, flag);
            
            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


