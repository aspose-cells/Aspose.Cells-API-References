---
title: "FontConfigs.GetFontFileDataInfo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FontConfigs yöntemi. Yazı tipi dosyası verisinin veri bilgilerini al"
type: docs
url: /tr/net/aspose.cells/fontconfigs/getfontfiledatainfo/
---
## FontConfigs.GetFontFileDataInfo method

Yazı tipi dosyası verisinin bilgi verilerini al.

```csharp
public static FontFileDataInfo GetFontFileDataInfo(string fontName, bool isBold, bool isItalic, 
    bool isExactStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fontName | String | yazı tipi adı |
| isBold | Boolean | yazı tipi stili kalın mı değil mi |
| isItalic | Boolean | yazı tipi stili italik mi değil mi |
| isExactStyle | Boolean | verilen kalın/italik stilini tam olarak eşleştirip eşleştirilmeyeceği |

### Dönüş Değeri

Yazı tipi dosyası verisinin veri bilgisi.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodGetFontFileDataInfoWithStringBooleanBooleanBooleanDemo
    {
        public static void Run()
        {
            try
            {
                // Belirli parametrelerle GetFontFileDataInfo yöntemini çağırın (statik çağrıya değiştirildi)
                FontFileDataInfo fontInfo = FontConfigs.GetFontFileDataInfo("Arial", true, false, false);

                // Yazı tipi dosyası verileri hakkında bilgi göster
                if (fontInfo != null)
                {
                    Console.WriteLine($"Font format type: {fontInfo.FormatType}");
                    Console.WriteLine($"Font data length: {fontInfo.Data?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Font information not available");
                }

                // Bir çalışma kitabı üzerindeki etkiyi göster
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Kontrol ettiğimiz yazı tipiyle stili ayarla
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.IsBold = true;
                style.Font.IsItalic = false;
                
                // Stili bir hücreye uygula
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text with Arial Bold");

                // Çalışma kitabını kaydedin
                workbook.Save("FontConfigsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontFileDataInfo method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontFileDataInfo](../../fontfiledatainfo/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


