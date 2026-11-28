---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageSaveOptions yapıcı. Görüntü dosyası kaydetmek için seçenekleri oluşturur"
type: docs
url: /tr/net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

Görüntü dosyasını kaydetmek için seçenekleri oluşturur.

```csharp
public ImageSaveOptions()
```

### Açıklamalar

Varsayılan tip Tiff'tir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ImageSaveOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için bazı veriler ekle
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Parametresiz yapıcıyı göster
                ImageSaveOptions defaultOptions = new ImageSaveOptions();
                Console.WriteLine("Created ImageSaveOptions with default constructor");

                // SaveFormat parametresiyle yapıcıyı göster
                ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
                Console.WriteLine("Created ImageSaveOptions with SaveFormat.Png");

                // Salt okunur ImageOrPrintOptions özelliğine eriş
                var imageOptions = pngOptions.ImageOrPrintOptions;
                Console.WriteLine($"ImageOrPrintOptions type: {imageOptions.GetType().Name}");

                // StreamProvider özelliğini ayarla
                pngOptions.StreamProvider = null;
                Console.WriteLine("StreamProvider set to null");

                // Oluşturulan seçeneklerle çalışma kitabını kaydet
                workbook.Save("output.png", pngOptions);
                Console.WriteLine("Workbook saved successfully with ImageSaveOptions");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

Görüntü dosyasını kaydetmek için seçenekleri oluşturur.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveFormat | SaveFormat | Dosya biçimi. Aşağıdaki türlerden biri olmalıdır: Tiff, Svg, Bmp, Png, Jpg, Emf veya Gif; aksi takdirde kaydedilen biçim otomatik olarak Tiff olarak ayarlanır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve test verileri ekleyin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
            
            // SaveFormat.Tiff ile ImageSaveOptions oluşturun
            try
            {
                ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
                
                // Görüntü işleme seçeneklerini yapılandırın
                saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
                saveOptions.ImageOrPrintOptions.VerticalResolution = 300;

                // Çalışma kitabını çok sayfalı TIFF olarak kaydedin
                workbook.Save("WorksheetImage.tiff", saveOptions);
                
                Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image save operation: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


