---
title: "PdfSaveOptions.ImageType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PdfSaveOptions özelliği. Grafik ve şekil dönüştürülürken görüntü tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/pdfsaveoptions/imagetype/
---
## PdfSaveOptions.ImageType property

Grafik ve şekil dönüştürülürken görüntü tipini temsil eder.

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ImageType { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanılmıyor. Bunun yerine, Chart ve Shape her zaman vektör öğeleri (ör. nokta, çizgi) olarak işlenir, bu da render kalitesini artırır. Bu özellik, Haziran 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing.Imaging;

    public class PdfSaveOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Bazı verilerle örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for PDF Export";
            worksheet.Cells["A2"].Value = "Demonstrating ImageType Property";

            try
            {
                // PDF kaydetme seçeneklerini oluşturun
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Varsayılan ImageType değerini gösterin
                Console.WriteLine("Default ImageType: " + saveOptions.ImageType);

                // Farklı bir ImageType değeri ayarlayın
                saveOptions.ImageType = ImageFormat.Png;
                Console.WriteLine("Updated ImageType: " + saveOptions.ImageType);

                // Çalışma kitabını belirtilen ImageType ile PDF olarak kaydedin
                workbook.Save("ImageTypeDemo.pdf", saveOptions);

                Console.WriteLine("PDF saved with ImageType setting applied.");
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

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


