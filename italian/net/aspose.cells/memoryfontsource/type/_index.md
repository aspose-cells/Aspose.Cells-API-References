---
title: "MemoryFontSource.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MemoryFontSource. Restituisce il tipo della font source"
type: docs
url: /it/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

Restituisce il tipo della fonte del font.

```csharp
public override FontSourceType Type { get; }
```

### Esempi

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
            // Carica un file di font TrueType in memoria
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Crea un'istanza MemoryFontSource con i dati del font
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Visualizza il valore corrente di Type
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le font source usando FontConfigs
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Verifica che il tipo della font source sia MemoryFont
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // Usa il font in una cella
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // Aggiungi informazioni sul tipo della font source
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // Salva la cartella di lavoro
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


