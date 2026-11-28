---
title: "ImageOrPrintOptions.SetDesiredSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImageOrPrintOptions yöntemi. Görüntünün istenen genişliğini ve yüksekliğini ayarlar"
type: docs
url: /tr/net/aspose.cells.rendering/imageorprintoptions/setdesiredsize/
---
## SetDesiredSize(int, int) {#setdesiredsize}

Görüntünün istenen genişlik ve yüksekliğini ayarlar.

```csharp
[Obsolete("Use SetDesiredSize(int, int, bool) by setting param keepAspectRatio to false instead.")]
public void SetDesiredSize(int desiredWidth, int desiredHeight)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desiredWidth | Int32 | piksellerde istenen genişlik |
| desiredHeight | Int32 | piksellerde istenen yükseklik |

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, `SetDesiredSize` yöntemini kullanarak keepAspectRatio parametresini false olarak ayarlayın. Bu özellik Mayıs 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue(i);
            }

            // Yazdırma alanını ayarla
            worksheet.PageSetup.PrintArea = "A1:A11";

            // Görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.SetDesiredSize(800, 600); // Using SetDesiredSize with Int32 parameters
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            // Çalışma sayfasını görüntüye dönüştür
            SheetRender render = new SheetRender(worksheet, options);
            render.ToImage(0, "output.jpg");

            Console.WriteLine("Image generated with desired size 800x600");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## SetDesiredSize(int, int, bool) {#setdesiredsize_1}

Görüntünün istenen genişlik ve yüksekliğini ayarlar.

```csharp
public void SetDesiredSize(int desiredWidth, int desiredHeight, bool keepAspectRatio)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| desiredWidth | Int32 | piksellerde istenen genişlik |
| desiredHeight | Int32 | piksellerde istenen yükseklik |
| keepAspectRatio | Boolean | orijinal görüntünün en-boy oranını koruyup korumayacağı |

### Açıklamalar

Çıktı görüntüsünün piksel cinsinden genişliği ve yüksekliği yalnızca ayarlanan istenen genişlik ve yüksekliğe dayanacaktır.

Bu durumda [`HorizontalResolution`](../horizontalresolution/) ve [`VerticalResolution`](../verticalresolution/) çıktının genişlik ve yüksekliğini etkilemeyecektir.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsMethodSetDesiredSizeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin ve bir grafik oluşturun
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Grafik şekli alın
            Shape chartShape = worksheet.Shapes[0];

            // Görüntü seçeneklerini ayarla
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            options.SetDesiredSize(800, 600, false); // Using SetDesiredSize with width, height, and keepAspectRatio

            // Grafiği görüntü olarak kaydet
            MemoryStream stream = new MemoryStream();
            chartShape.ToImage(stream, options);

            // Görüntüyü dosyaya kaydet
            File.WriteAllBytes("output_chart.png", stream.ToArray());
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


