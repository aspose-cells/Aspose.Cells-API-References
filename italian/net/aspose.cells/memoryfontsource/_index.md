---
title: "Classe MemoryFontSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.MemoryFontSource. Rappresenta il singolo file di font TrueType memorizzato in memoria"
type: docs
url: /it/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

Rappresenta il singolo file di font TrueType memorizzato in memoria.

```csharp
public class MemoryFontSource : FontSourceBase
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Ctor. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | Dati binari del font. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Restituisce il tipo della fonte del font. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Carica un file di font TrueType in memoria
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Crea un'istanza di MemoryFontSource con i dati del font
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Crea un array di font source contenente la nostra MemoryFontSource
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // Imposta le font source usando FontConfigs
            FontConfigs.SetFontSources(fontSources);

            // Usa il font personalizzato in una cella
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


