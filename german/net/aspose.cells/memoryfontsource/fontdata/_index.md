---
title: "MemoryFontSource.FontData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MemoryFontSource-Eigenschaft. Binäre Schriftartdaten"
type: docs
url: /de/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

Binäre Schriftartdaten.

```csharp
public byte[] FontData { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyFontDataDemo
    {
        public static void Run()
        {
            // Lade eine TrueType-Schriftdatei in den Speicher
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // Erstellen Sie eine MemoryFontSource-Instanz mit den Schriftartdaten
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // Aktuellen FontData-Wert anzeigen (erste 10 Bytes zur Demonstration)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Schrifteinstellungen erstellen und unsere MemoryFontSource hinzufügen
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Schriftkonfigurationen global anwenden (nicht arbeitsmappen-spezifisch)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Erstellen Sie einen Stil mit der benutzerdefinierten Schriftart
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // Wende den Stil auf eine Zelle an
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // Speichere die Arbeitsmappe
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


