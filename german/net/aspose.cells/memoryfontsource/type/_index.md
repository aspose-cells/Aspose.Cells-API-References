---
title: "MemoryFontSource.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MemoryFontSource-Eigenschaft. Gibt den Typ der Schriftquelle zurück"
type: docs
url: /de/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

Gibt den Typ der Schriftquellen zurück.

```csharp
public override FontSourceType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            // Lade eine TrueType-Schriftdatei in den Speicher
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Erstellen Sie eine MemoryFontSource-Instanz mit den Schriftartdaten
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Aktuellen Type-Wert anzeigen
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Schriftquellen mit FontConfigs festlegen
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Überprüfen Sie, dass der Schriftquellentyp MemoryFont ist
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // Verwenden Sie die Schriftart in einer Zelle
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // Informationen zum Schriftquellentyp hinzufügen
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


