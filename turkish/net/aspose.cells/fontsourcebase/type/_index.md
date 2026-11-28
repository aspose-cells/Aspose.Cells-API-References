---
title: "FontSourceBase.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontSourceBase özelliği. Font kaynağının tipini döndürür"
type: docs
url: /tr/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

Yazı tipi kaynağının türünü döndürür.

```csharp
public abstract FontSourceType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı örneği oluştur
            Workbook workbook = new Workbook();
            
            // Klasör yazı tipi kaynağı oluştur
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // Font kaynağının Type özelliğini göster
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // Bir dosya font kaynağı oluştur
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // Font kaynağının Type özelliğini göster
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // Bellek font kaynağı oluştur (bayt dizisi örneği)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // Font kaynağının Type özelliğini göster
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // Statik yöntemi kullanarak font kaynaklarını ayarla
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // Çalışma kitabını kaydedin
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


