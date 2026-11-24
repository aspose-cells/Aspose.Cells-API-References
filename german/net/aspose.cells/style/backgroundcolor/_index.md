---
title: "Style.BackgroundColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt die Hintergrundfarbe eines Stils zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Liest oder setzt die Hintergrundfarbe eines Stils.

```csharp
public Color BackgroundColor { get; set; }
```

### Hinweise

Wenn Sie die Farbe einer Zelle festlegen möchten, verwenden Sie bitte die Style.ForegroundColor-Eigenschaft. Nur wenn das Zellenstil-Muster nicht 'none' oder 'solid' ist, wird diese Eigenschaft wirksam.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie ein Stilobjekt
            Style style = workbook.CreateStyle();
            
            // Hintergrundfarbe auf Gelb setzen
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Den Stil auf Zelle A1 anwenden
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


