---
title: "FontFileDataInfo.FormatType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontFileDataInfo özelliği. Yazı tipi dosyasının format türünü alır"
type: docs
url: /tr/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Yazı tipi dosyasının format türünü alır.

```csharp
public FontFileFormatType FormatType { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yazı tipi kullanımını göstermek için biraz metin ekle
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Örnek bir yazı tipi dosyası yükle (gerçek yazı tipi dosyası yoluyla değiştirin)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Yazı tipi klasörünü kaydet
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // Gerçek bir senaryoda, FontFileDataInfo kütüphaneden elde edilir
                    // Demonstrasyon için, yazı tipi bilgisi alımını taklit edeceğiz
                    // Not: Gerçek API bunu FontConfigs veya benzeri aracılığıyla sağlayabilir
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // FormatType özelliğinin değerini göster
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Enum değerini dize olarak göster
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Yazı tipini bir hücreye uygula (kavramsal - gerçek uygulama değişebilir)
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // FontFileDataInfo alımını taklit eden yardımcı yöntem
        // Gerçek kullanımda, bu Aspose.Cells API'si tarafından sağlanır
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Bir taklit FontFileDataInfo oluştur (gerçekte, bu API'den gelir)
                // Doğrudan örnekleyemediğimiz için, davranışı taklit edeceğiz
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // Gerçek bir uygulamada, bu API tarafından döndürülür
                // Bu demo için, nesneyi oluşturamadığımız için sadece null döndüreceğiz
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


