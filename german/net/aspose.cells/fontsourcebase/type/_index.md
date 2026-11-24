---
title: "FontSourceBase.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSourceBase-Eigenschaft. Gibt den Typ der Schriftquellen zurück"
type: docs
url: /de/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

Gibt den Typ der Schriftquellen zurück.

```csharp
public abstract FontSourceType Type { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappeninstanz
            Workbook workbook = new Workbook();
            
            // Erstelle eine Ordner‑Schriftquelle
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // Zeigen Sie die Type-Eigenschaft der Schriftquelle an
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // Erstelle eine Schriftartquelle aus Datei
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // Zeigen Sie die Type-Eigenschaft der Schriftquelle an
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // Erstelle eine Speicher‑Schriftartquelle (Beispiel mit Byte‑Array)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // Zeigen Sie die Type-Eigenschaft der Schriftquelle an
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // Setze Schriftartquellen mithilfe der statischen Methode
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


