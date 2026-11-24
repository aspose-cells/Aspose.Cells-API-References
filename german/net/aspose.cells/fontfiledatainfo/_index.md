---
title: "Klasse FontFileDataInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontFileDataInfo Klasse. Stellt Dateninformationen von Schriftdateidaten dar"
type: docs
url: /de/net/aspose.cells/fontfiledatainfo/
---
## FontFileDataInfo class

Stellt Dateninformationen von Schriftdateidaten dar.

```csharp
public class FontFileDataInfo
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Data](../../aspose.cells/fontfiledatainfo/data/) { get; } | Liest Binärdaten der Schriftdatei. |
| [FormatType](../../aspose.cells/fontfiledatainfo/formattype/) { get; } | Liest Schriftformattyp der Schriftdatei. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassFontFileDataInfoDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispiel: Laden von Schriftdateidaten
            string fontFilePath = "arial.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Hinweis: FontFileDataInfo kann nicht direkt instanziiert werden, da es keinen öffentlichen Konstruktor hat
            // und seine Eigenschaften sind schreibgeschützt. In einem realen Szenario würden Sie eine Instanz erhalten
            // aus einer anderen API-Methode (wie FontConfigs.GetFontFileDataInfo())
            FontFileDataInfo fontInfo = null; // Would be populated by API call in real scenario

            // Demonstriere, wie Eigenschaften verwendet würden, wenn wir eine Instanz hätten
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
                Console.WriteLine("Font data length: " + (fontInfo.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            }

            // Demonstriere die Integration mit Workbook
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with custom font");

            // Speichere die Arbeitsmappe
            workbook.Save("FontFileDataInfoDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


