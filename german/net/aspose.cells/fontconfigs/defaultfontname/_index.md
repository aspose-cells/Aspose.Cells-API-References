---
title: "FontConfigs.DefaultFontName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Eigenschaft. Liest oder setzt den Standard-Schriftnamen"
type: docs
url: /de/net/aspose.cells/fontconfigs/defaultfontname/
---
## FontConfigs.DefaultFontName property

Liest oder legt den Standard-Schriftartnamen fest.

```csharp
public static string DefaultFontName { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aktuellen Standard-Schriftnamen anzeigen
            Console.WriteLine("Current DefaultFontName value: " + FontConfigs.DefaultFontName);

            // Neuen Standard-Schriftnamen festlegen
            FontConfigs.DefaultFontName = "Arial";

            // Erstellen Sie einen Stil ohne explizite Schrift, um die Verwendung der Standardschrift zu demonstrieren
            Style style = workbook.CreateStyle();
            style.Font.Name = ""; // Empty to use default font

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text should use the default font");
            cell.SetStyle(style);

            // Speichern Sie die Arbeitsmappe, um den Effekt zu sehen
            workbook.Save("PropertyDefaultFontNameDemo.xlsx");

            // Überprüfen Sie, ob die Schrift korrekt angewendet wurde
            Console.WriteLine("Cell font after setting DefaultFontName: " + cell.GetStyle().Font.Name);
        }
    }
}
```

### Siehe auch

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


