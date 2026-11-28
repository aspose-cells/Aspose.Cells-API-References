---
title: "PageSetup.SetHeaderPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Çalışma sayfasının başlığına bir resim ayarlar"
type: docs
url: /tr/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

Çalışma sayfasının üstbilgisinde bir görüntü ayarlar.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| headerPicture | Byte[] | Görüntü verisi. |

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

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir görüntü dosyasını bayt dizisine yükle
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // SetHeaderPicture'ı bölüm indeksi (ortadaki başlık için 0) ve resim baytlarıyla çağır
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // Resmi göstermek için başlık betiğini ayarla
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


