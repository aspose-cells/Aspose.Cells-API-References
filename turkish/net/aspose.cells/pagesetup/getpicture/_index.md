---
title: "PageSetup.GetPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup yöntemi. Üstbilgi / altbilgi için Picture nesnesini alır"
type: docs
url: /tr/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Üstbilgi / altbilgi için [`Picture`](../../../aspose.cells.drawing/picture/) nesnesini alır.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isHeader | Boolean | Üstbilgide mi yoksa altbilgide mi olduğunu gösterir. |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

### Dönüş Değeri

Returns [`Picture`](../../../aspose.cells.drawing/picture/) nesnesini döndürür. Resim yoksa null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasının üstbilgisine bir resim ekleyin
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // Üstbilgiden resmi al ve parlaklığını değiştir
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Üstbilgi / altbilgi için [`Picture`](../../../aspose.cells.drawing/picture/) nesnesini alır.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isFirst | Boolean | İlk sayfa üstbilgi/altbilgi resmini alıp almadığını gösterir. |
| isEven | Boolean | Çift sayfa üstbilgi/altbilgi resmini alıp almadığını gösterir. |
| isHeader | Boolean | Üstbilgi/altbilgi resmini alıp almadığını gösterir. |
| bölüm | Int32 | 0: Sol Bölüm, 1: Orta Bölüm, 2: Sağ Bölüm. |

### Dönüş Değeri

[`Picture`](../../../aspose.cells.drawing/picture/) nesnesini döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // PageSetup nesnesini al
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Alınacak resimler olduğundan emin olmak için bazı üstbilgi/altbilgi özelliklerini ayarlayın
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // GetPicture yöntemini şu parametrelerle çağırın: isFirst, isEven, isHeader, section
                // İlk sayfa başlığı kontrol ediliyor (bölüm 0 - orta başlık)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
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


