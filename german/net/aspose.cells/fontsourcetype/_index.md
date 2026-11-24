---
title: "Enum FontSourceType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontSourceType enum. Gibt den Typ einer Schriftquelle an."
type: docs
url: /de/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Gibt den Typ einer Schriftartquelle an.

```csharp
public enum FontSourceType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| FontFile | `0` | repräsentiert eine einzelne Schriftdatei. |
| FontsFolder | `1` | Repräsentiert einen Ordner mit Schriftdateien. |
| MemoryFont | `2` | Repräsentiert eine einzelne Schrift im Speicher. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstriere FontSourceType-Enum-Werte
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Erstelle Schriftarteinstellungen und verwende FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Schrift auf eine Zelle anwenden
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Ergebnis speichern
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


