---
title: "WorkbookRender.ToImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookRender yöntemi. Tüm çalışma kitabını akışa Tiff Görüntüsü olarak render et."
type: docs
url: /tr/net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

Tüm çalışma kitabını Tiff Görüntüsü olarak akıma render eder.

```csharp
public void ToImage(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | çıktı görüntüsünün akışı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithStreamDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // Görüntü işleme seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // Çıktı dizini yoksa oluştur
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // Görüntü çıktısı için bir dosya akışı oluştur
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // Çalışma kitabı renderlayıcısını başlat ve görüntüye dönüştür
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // Referans için orijinal çalışma kitabını kaydet
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

Tüm çalışma kitabını Tiff Görüntüsü olarak bir dosyaya render eder.

```csharp
public void ToImage(string filename)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | String | çıktı görüntüsünün dosya adı |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // Görüntü seçeneklerini ayarla
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // Çalışma kitabı renderı oluştur ve görüntü olarak kaydet
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

Belirli bir sayfayı bir dosyaya render eder.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| fileName | String | çıktı görüntüsünün dosya adı |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // Çalışma kitabı render'ı oluştur
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Her sayfayı görüntü olarak kaydet
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

Belirli bir sayfayı akıma render eder.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| akış | Stream | çıktı görüntüsünün akışı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index and Stream Demo";

            // Görüntü işleme seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            try
            {
                // Çalışma kitabı renderlayıcısını başlat
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // İlk sayfa indeksini al (0 tabanlı)
                int pageIndex = 0;

                // Görüntüyü tutmak için bir bellek akışı oluştur
                using (MemoryStream stream = new MemoryStream())
                {
                    // Sayfa indeksi ve akış ile ToImage'i çağır
                    renderer.ToImage(pageIndex, stream);

                    // Sonuçları göster
                    Console.WriteLine($"Page {pageIndex} rendered successfully to stream");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");
                    Console.WriteLine($"Total pages available: {renderer.PageCount}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Belirli bir sayfayı Bitmap nesnesine render eder.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |

### Dönüş Değeri

sayfanın bitmap nesnesi

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index Demo";

            // Görüntü işleme seçeneklerini yapılandırın
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

            // Çıktı dizini yoksa oluştur
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            try
            {
                // Çalışma kitabı renderlayıcısını başlat
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // İlk sayfa indeksini al (0 tabanlı)
                int pageIndex = 0;

                // Sayfa indeksi ile ToImage'i çağır ve dosyaya kaydet
                string imagePath = Path.Combine(outputDir, $"page_{pageIndex}.png");
                renderer.ToImage(pageIndex, imagePath);

                Console.WriteLine($"Page {pageIndex} rendered successfully to: {imagePath}");
                Console.WriteLine($"Total pages available: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


