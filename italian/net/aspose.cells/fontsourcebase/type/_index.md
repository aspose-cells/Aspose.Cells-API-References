---
title: "FontSourceBase.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSourceBase. Restituisce il tipo della sorgente del carattere"
type: docs
url: /it/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

Restituisce il tipo della fonte del font.

```csharp
public abstract FontSourceType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un'istanza di cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Crea una fonte di font da cartella
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // Visualizza la proprietà Type della sorgente del carattere
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // Crea una sorgente di carattere da file
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // Visualizza la proprietà Type della sorgente del carattere
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // Crea una sorgente di carattere in memoria (esempio con array di byte)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // Visualizza la proprietà Type della sorgente del carattere
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // Imposta le sorgenti dei caratteri usando il metodo statico
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // Salva la cartella di lavoro
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


