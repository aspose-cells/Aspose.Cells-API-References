---
title: "Style.IsTextWrapped"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob der Text innerhalb einer Zelle umgebrochen ist"
type: docs
url: /de/net/aspose.cells/style/istextwrapped/
---
## Style.IsTextWrapped property

Liest oder setzt einen Wert, der angibt, ob der Text innerhalb einer Zelle umgebrochen wird.

```csharp
public bool IsTextWrapped { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;
            
            // Langen Text in einer Zelle festlegen
            Cell cell = cells["A1"];
            cell.PutValue("This is a long text that should be wrapped in the cell");
            
            // Textumbruch aktivieren
            Style style = cell.GetStyle();
            style.IsTextWrapped = true;
            cell.SetStyle(style);
            
            // Zeilenhöhe anpassen, um umgebrochenen Text anzuzeigen
            ws.AutoFitRow(0);
            
            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


