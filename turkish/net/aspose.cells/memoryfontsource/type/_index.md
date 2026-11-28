---
title: "MemoryFontSource.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MemoryFontSource özelliği. Yazı tipi kaynağının tipini döndürür"
type: docs
url: /tr/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

Yazı tipi kaynağının türünü döndürür.

```csharp
public override FontSourceType Type { get; }
```

### Örnekler

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
            // Bir TrueType yazı tipi dosyasını belleğe yükleyin
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Yazı tipi verisiyle bir MemoryFontSource örneği oluştur
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Mevcut Type değerini göster
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // FontConfigs kullanarak yazı tipi kaynaklarını ayarla
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Yazı tipi kaynağı tipinin MemoryFont olduğunu doğrula
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // Yazı tipini bir hücrede kullan
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // Yazı tipi kaynağı tipi hakkında bilgi ekle
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


