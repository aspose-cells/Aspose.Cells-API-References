---
title: "Klasse CellRichValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellRichValue-Klasse. Stellt den Rich-Wert der Zelle dar"
type: docs
url: /de/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Stellt den Rich-Wert der Zelle dar.

```csharp
public abstract class CellRichValue
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Liest den alternativen Text, der mit dem Bild verknüpft ist. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Liest den Fehlertypwert der Zelle. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Liest die Bilddaten der Zelle. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzt einen Rich-Wert in Zelle A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // Liest den Rich-Wert aus Zelle A1
            CellRichValue richValue = cell.GetRichValue();
            
            // Zeigt die Eigenschaften des Rich-Werts an
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Speichere die Arbeitsmappe
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


