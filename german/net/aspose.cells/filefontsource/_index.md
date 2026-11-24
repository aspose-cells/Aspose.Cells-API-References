---
title: "Klasse FileFontSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FileFontSource Klasse. Stellt die einzelne TrueType-Schriftdatei dar, die im Dateisystem gespeichert ist"
type: docs
url: /de/net/aspose.cells/filefontsource/
---
## FileFontSource class

Stellt die einzelne TrueType‑Schriftdatei dar, die im Dateisystem gespeichert ist.

```csharp
public class FileFontSource : FontSourceBase
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Ctor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Pfad zur Schriftdatei. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Gibt den Typ der Schriftquellen zurück. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // Gib den Pfad zur TrueType-Schriftdatei an
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // Erstelle eine FileFontSource-Instanz
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Zeige den Schriftquellentyp und den Dateipfad an
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Erstelle ein Workbook-Objekt
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Setze einen Zellenwert
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Wende die benutzerdefinierte Schriftart auf die Zelle an
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### Siehe auch

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


