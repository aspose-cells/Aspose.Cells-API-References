---
title: "MemoryFontSource.MemoryFontSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "MemoryFontSource yapıcı. Ctor"
type: docs
url: /tr/net/aspose.cells/memoryfontsource/memoryfontsource/
---
## MemoryFontSource constructor

Yapıcı.

```csharp
public MemoryFontSource(byte[] fontData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontData | Byte[] | İkili yazı tipi verisi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourceMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // TrueType yazı tipi dosyasını bayt dizisine yükle
                byte[] fontData = File.ReadAllBytes("arial.ttf");
                
                // Bayt dizisi parametresiyle #ctor metodunu çağır
                MemoryFontSource fontSource = new MemoryFontSource(fontData);
                
                // FontConfigs statik sınıfını kullanarak yazı tipi kaynaklarını ayarla
                FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
                
                // Yazı tipi kaynaklarını doğrula
                Console.WriteLine($"Font source type: {fontSource.Type}");
                Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
                
                // Yazı tipini bir hücrede kullan
                Worksheet worksheet = workbook.Worksheets[0];
                var style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].PutValue("Text with custom font");
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("MemoryFontSource constructor executed successfully with byte array parameter");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error: Font file not found. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MemoryFontSource constructor: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MemoryFontSourceCtorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


