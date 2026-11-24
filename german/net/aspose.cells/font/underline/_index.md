---
title: "Font.Underline"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schriftart-Eigenschaft. Gibt den Unterstreichungs-Typ der Schriftart zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/font/underline/
---
## Font.Underline property

Liest oder setzt den Unterstreichungstyp der Schriftart.

```csharp
public FontUnderlineType Underline { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyUnderlineDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Greifen Sie auf die Zelle zu und setzen Sie den Unterstreichungsstil
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Underlined Text");
            
            // Holen Sie den Stil und ändern Sie die Schriftarteigenschaften
            Style style = cell.GetStyle();
            style.Font.Underline = FontUnderlineType.Single;
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FontUnderlineType](../../fontunderlinetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


