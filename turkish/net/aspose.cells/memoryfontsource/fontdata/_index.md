---
title: "MemoryFontSource.FontData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MemoryFontSource özelliği. İkili yazı tipi verileri"
type: docs
url: /tr/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

İkili yazı tipi verisi.

```csharp
public byte[] FontData { get; }
```

### Örnekler

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
            // Bir TrueType yazı tipi dosyasını belleğe yükleyin
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // Yazı tipi verisiyle bir MemoryFontSource örneği oluştur
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // Mevcut FontData değerini göster (gösterim için ilk 10 bayt)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yazı tipi ayarlarını oluştur ve bellek yazı tipi kaynağımızı ekle
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Yazı tipi yapılandırmalarını global olarak uygula (çalışma kitabına özgü değil)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Özel yazı tipiyle bir stil oluştur
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // Stili bir hücreye uygula
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // Çalışma kitabını kaydedin
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


