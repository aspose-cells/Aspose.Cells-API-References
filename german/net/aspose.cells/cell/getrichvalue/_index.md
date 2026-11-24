---
title: "Cell.GetRichValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt den Rich-Wert der Zelle zurück"
type: docs
url: /de/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Liefert den Rich‑Wert der Zelle.

```csharp
public CellRichValue GetRichValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet ws = wb.Worksheets[0];
            
            // Rich-Text-Wert in Zelle A1 festlegen
            ws.Cells["A1"].PutValue("This is rich text");
            
            // Liest den Rich-Wert aus Zelle A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Rich-Text-Wert anzeigen
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Speichere die Arbeitsmappe
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


