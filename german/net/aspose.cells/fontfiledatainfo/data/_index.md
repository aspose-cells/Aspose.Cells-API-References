---
title: "FontFileDataInfo.Data"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontFileDataInfo-Eigenschaft. Gibt die Binärdaten der Schriftdatei zurück"
type: docs
url: /de/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

Liest Binärdaten der Schriftdatei.

```csharp
public byte[] Data { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Lade eine Schriftdatei (ersetze durch den tatsächlichen Pfad zur Schriftdatei)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Erstelle eine FontConfigs-Instanz und füge die Schriftart hinzu
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // Im realen Einsatz würde FontFileDataInfo aus der Bibliothek erhalten werden
            // Zu Demonstrationszwecken zeigen wir nur, wie du es verwenden würdest, wenn du eines hättest
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // Zeige Informationen über die Schriftartdaten an (falls verfügbar)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // Im realen Einsatz würde die Data-Eigenschaft verwendet werden, um auf die Binärdaten der Schriftart zuzugreifen
            // Zum Beispiel könntest du es in einer Datei speichern:
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // Speichere die Arbeitsmappe (die Schriftart würde das Rendering beeinflussen, wenn sie in Zellen verwendet wird)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


