---
title: "FontFileDataInfo.Data"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontFileDataInfo özelliği. Yazı tipi dosyasının ikili verilerini alır"
type: docs
url: /tr/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

Yazı tipi dosyasının ikili verilerini alır.

```csharp
public byte[] Data { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir yazı tipi dosyası yükle (gerçek yazı tipi dosyası yoluyla değiştirin)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Bir FontConfigs örneği oluştur ve yazı tipini ekle
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // Gerçek kullanımda, FontFileDataInfo kütüphaneden elde edilir
            // Demonstrasyon amaçları için, eğer bir tane olsaydı nasıl kullanacağınızı sadece göstereceğiz
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // Yazı tipi verileri hakkında bilgiyi göster (varsa)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // Gerçek kullanımda, Data özelliği yazı tipi ikili verilerine erişmek için kullanılır
            // Örneğin, bunu bir dosyaya kaydedebilirsiniz:
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // Çalışma kitabını kaydet (yazı tipi hücrelerde kullanılırsa renderlamayı etkiler)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


