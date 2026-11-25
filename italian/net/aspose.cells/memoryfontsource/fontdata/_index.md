---
title: "MemoryFontSource.FontData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MemoryFontSource. Dati binari del font"
type: docs
url: /it/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

Dati binari del font.

```csharp
public byte[] FontData { get; }
```

### Esempi

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
            // Carica un file di font TrueType in memoria
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // Crea un'istanza MemoryFontSource con i dati del font
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // Visualizza il valore corrente di FontData (primi 10 byte per dimostrazione)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea le impostazioni del font e aggiungi la nostra fonte di font in memoria
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Applica le configurazioni del font a livello globale (non specifiche del workbook)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Crea uno stile con il font personalizzato
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // Applica lo stile a una cella
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // Salva la cartella di lavoro
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


