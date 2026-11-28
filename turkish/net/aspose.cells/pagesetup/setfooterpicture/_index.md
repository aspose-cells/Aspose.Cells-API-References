---
title: "PageSetup.SetFooterPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Bir çalışma sayfasının altbilgi kısmına bir görüntü ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

Çalışma sayfasının altbilgisinde bir görüntü ayarlar.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| footerPicture | Byte[] | Görüntü verisi. |

### Dönüş Değeri

[`Picture`](../../../aspose.cells.drawing/picture/) nesnesini döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir görüntü dosyasını bayt dizisine yükle
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // SetFooterPicture yöntemini bölüm indeksi (0 ortada, 1 solda, 2 sağda) ve görüntü verisi ile çağırın
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // Görüntüyle birlikte gösterilecek altbilgi metnini ayarlayın
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // Altbilgi görüntüsünü görmek için çalışma kitabını kaydedin
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


