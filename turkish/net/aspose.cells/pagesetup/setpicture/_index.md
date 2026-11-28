---
title: "PageSetup.SetPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Çalışma sayfasının başlık/altbilgisine bir resim ayarlar."
type: docs
url: /tr/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

Çalışma sayfasının üstbilgi/altbilgisinde bir görüntü ayarlar.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isFirst | Boolean | İlk sayfa başlık/altbilgisinin resmini ayarlayıp ayarlamadığını gösterir. |
| isEven | Boolean | Çift sayfa başlık/altbilgisinin resmini ayarlayıp ayarlamadığını gösterir. |
| isHeader | Boolean | Başlık/altbilgi resmini ayarlayıp ayarlamadığını gösterir. |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |
| imageData | Byte[] | Görüntü verisi. |

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

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Bir görüntü dosyasını bayt dizisine yükle
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // Üstbilgi resmini ayarlamak için SetPicture yöntemini çağır
                // Parametreler: isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // Üstbilgi metnini ayarla
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // Çalışma kitabını kaydedin
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
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


