---
title: "Klasse MemoryFontSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.MemoryFontSource-Klasse. Stellt die einzelne TrueType-Schriftdatei dar, die im Speicher gespeichert ist"
type: docs
url: /de/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

Stellt die einzelne TrueType-Schriftdatei dar, die im Speicher gespeichert ist.

```csharp
public class MemoryFontSource : FontSourceBase
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Ctor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | Binäre Schriftartdaten. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Gibt den Typ der Schriftquellen zurück. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassMemoryFontSourceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lade eine TrueType-Schriftdatei in den Speicher
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Erstelle eine Instanz von MemoryFontSource mit den Schriftartdaten
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Erstelle ein Array von Schriftquellen, das unsere MemoryFontSource enthält
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // Setze die Schriftquellen mithilfe von FontConfigs
            FontConfigs.SetFontSources(fontSources);

            // Verwende die benutzerdefinierte Schriftart in einer Zelle
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


