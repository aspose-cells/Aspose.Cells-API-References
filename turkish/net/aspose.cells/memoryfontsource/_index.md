---
title: "MemoryFontSource sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.MemoryFontSource sınıfı. Bellekte depolanan tek TrueType yazı tipi dosyasını temsil eder"
type: docs
url: /tr/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

Bellekte depolanan tek TrueType yazı tipi dosyasını temsil eder.

```csharp
public class MemoryFontSource : FontSourceBase
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | İkili yazı tipi verisi. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Yazı tipi kaynağının türünü döndürür. |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir TrueType yazı tipi dosyasını belleğe yükleyin
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Yazı tipi verisiyle bir MemoryFontSource örneği oluşturun
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Bellek yazı tipi kaynağımızı içeren yazı tipi kaynakları dizisi oluşturun
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // FontConfigs kullanarak yazı tipi kaynaklarını ayarlayın
            FontConfigs.SetFontSources(fontSources);

            // Bir hücrede özel yazı tipini kullanın
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


