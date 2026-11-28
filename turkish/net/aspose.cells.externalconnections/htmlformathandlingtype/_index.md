---
title: "Enum HtmlFormatHandlingType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.HtmlFormatHandlingType enum. HTML kaynağından gelen biçimlendirmeyi nasıl ele alacağını belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/htmlformathandlingtype/
---
## HtmlFormatHandlingType enumeration

HTML kaynağından gelen biçimlendirmeyi nasıl ele alacağını belirtir

```csharp
public enum HtmlFormatHandlingType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| All | `0` | Tüm HTML biçimlendirmesini veriyle birlikte çalışma sayfasına aktar. |
| None | `1` | Veriyi biçimlendirilmemiş metin olarak getir (veri tipleri hâlâ ayarlanır). |
| Rtf | `2` | HTML biçimlendirmesini, çalışma sayfasına getirilen veride zengin metin biçimlendirmesine çevir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassHtmlFormatHandlingTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // HtmlFormatHandlingType enum değerlerinin tümünü göster
                HtmlFormatHandlingType allFormatting = HtmlFormatHandlingType.All;
                HtmlFormatHandlingType noFormatting = HtmlFormatHandlingType.None;
                HtmlFormatHandlingType rtfFormatting = HtmlFormatHandlingType.Rtf;

                // Enum değerlerini görüntüle
                Console.WriteLine("HtmlFormatHandlingType.All: " + allFormatting);
                Console.WriteLine("HtmlFormatHandlingType.None: " + noFormatting);
                Console.WriteLine("HtmlFormatHandlingType.Rtf: " + rtfFormatting);

                // Bu değerleri bir senaryoda kullanarak simüle et
                worksheet.Cells["A1"].PutValue("Format Handling Types:");
                worksheet.Cells["A2"].PutValue("All Formatting");
                worksheet.Cells["A3"].PutValue("No Formatting");
                worksheet.Cells["A4"].PutValue("RTF Formatting");

                // Çalışma kitabını kaydedin
                workbook.Save("HtmlFormatHandlingTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in HtmlFormatHandlingType demo: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


