---
title: "Cell.HtmlString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt den html-String zurück und setzt ihn, der Daten und einige Formate in dieser Zelle enthält."
type: docs
url: /de/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Liefert und setzt die HTML‑Zeichenkette, die Daten und einige Formate in dieser Zelle enthält.

```csharp
public string HtmlString { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappeninstanz
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Auf die Cells-Sammlung zugreifen
            Cells cells = worksheet.Cells;
            
            // HTML-String mit Formatierung in Zelle A1 setzen
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // Speichere die Arbeitsmappe
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


