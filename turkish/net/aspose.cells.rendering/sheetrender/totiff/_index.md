---
title: "SheetRender.ToTiff"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetRender yöntemi. Tüm çalışma sayfasını Tiff görüntüsü olarak akıma render edin"
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Tüm çalışma sayfasını Tiff Image olarak akışa render et.

```csharp
public void ToTiff(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | çıktı görüntüsünün akışı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToTiffWithStreamDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Render etmeyi göstermek için örnek içerik ekleyin
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // Render için görüntü seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Yapılandırılmış seçeneklerle sayfa renderlayıcısını oluşturun
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // TIFF görüntüsü için çıktı akışı oluşturun
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // Akışı kullanarak çalışma sayfasını TIFF olarak render edin
                    renderer.ToTiff(tiffStream);
                    Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Tüm çalışma sayfasını Tiff Image olarak bir dosyaya render et.

```csharp
public void ToTiff(string filename)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | String | çıktı görüntüsünün dosya adı |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToTiffWithStringDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasını yükle
            Workbook workbook = new Workbook("Book1.xlsx");

            // Görüntü veya yazdırma seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // İlk çalışma sayfası için sayfa renderi oluştur
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // Sayfanın tüm sayfalarını çok sayfalı bir TIFF dosyası olarak kaydedin
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


