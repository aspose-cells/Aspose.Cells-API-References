---
title: "Enum ImageBinarizationMethod"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.ImageBinarizationMethod enum. Görüntüyü ikili hale getirmek için kullanılan yöntemi belirtir"
type: docs
url: /tr/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

Görüntüyü ikili hale getirmek için kullanılan yöntemi belirtir.

```csharp
public enum ImageBinarizationMethod
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Threshold | `0` | Eşik yöntemini belirtir. |
| FloydSteinbergDithering | `1` | Floyd-Steinberg hata yayılımı yöntemi kullanarak titreme işlemini belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // Test verileriyle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gösterim için hücreleri degrade değerlerle doldurun
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // Görüntü işleme seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // Yapılandırılmış seçeneklerle sayfa işleme oluşturun
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // İlk çalışma sayfasını ikili hale getirerek görüntüye işleyin
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


