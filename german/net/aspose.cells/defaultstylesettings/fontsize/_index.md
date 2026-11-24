---
title: "DefaultStyleSettings.FontSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DefaultStyleSettings-Eigenschaft. Gibt/Setzt die standardmäßige Standardschriftgröße für die Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

Liest/Setzt die Standard‑Schriftgröße für die Arbeitsmappe.

```csharp
public double FontSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // Standard‑Schriftartnamen und -größe festlegen
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // HTML-Datei mit diesen Einstellungen laden
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // Auf eine Zelle zugreifen und deren Schriftgröße anzeigen
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### Siehe auch

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


