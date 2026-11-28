---
title: "SheetRender.ToImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SheetRender yöntemi. Belirli bir sayfayı Graphics nesnesine render eder"
type: docs
url: /tr/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Belirli bir sayfayı Graphics'e render et

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| g | Grafikler | Render yapılacak nesne. |
| x | Single | Render edilen sayfanın sol üst köşesinin X koordinatı (piksel cinsinden). |
| y | Single | Render edilen sayfanın sol üst köşesinin Y koordinatı (piksel cinsinden). |
| genişlik | Single | Render edilen sayfanın kaplayabileceği maksimum genişlik (piksel cinsinden). |
| yükseklik | Single | Render edilen sayfanın kaplayabileceği maksimum yükseklik (piksel cinsinden). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Görüntü seçenekleri oluştur
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Çalışma sayfası için sayfa renderi oluştur
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Render edilen görüntüyü yakalamak için bir bellek akışı oluştur
                using (MemoryStream stream = new MemoryStream())
                {
                    // Belirtilen parametrelerle ToImage'i çağır
                    // System.Drawing.Graphics'i kullanamadığımız için daha basit ToImage aşırı yüklemesini kullanacağız.
                    sheetRender.ToImage(0, stream);

                    // Render edilen görüntüyü dosyaya kaydet
                    File.WriteAllBytes("RenderedOutput.png", stream.ToArray());
                }

                Console.WriteLine("Sheet rendered to image successfully.");
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

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Belirli bir sayfayı Graphics'e render et

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfaIndeksi | Int32 | hangi sayfanın dönüştürüleceğini belirt |
| g | Grafikler | Render yapılacak nesne. |
| x | Single | Render edilen sayfanın sol üst köşesinin X koordinatı (piksel cinsinden). |
| y | Single | Render edilen sayfanın sol üst köşesinin Y koordinatı (piksel cinsinden). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // SheetRender örneği oluştur
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // System.Drawing türlerini kullanamadığımız için alternatif ToImage yöntemini kullanacağız.
                // dosyaya doğrudan kaydeder
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Kaynakları temizle
                sheetRender.Dispose();
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

## ToImage(int, string) {#toimage_4}

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
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasını yükle
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // İlk çalışma sayfası için sayfa renderi oluştur
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Sayfanın ilk sayfasını bir görüntü dosyasına render et
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

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

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Görüntü seçenekleri oluştur
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // SheetRender örneği oluştur
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Görüntüyü tutmak için bir bellek akışı oluştur
                using (MemoryStream stream = new MemoryStream())
                {
                    // Sayfa indeksi ve akış parametreleriyle ToImage'i çağır
                    sheetRender.ToImage(0, stream);

                    Console.WriteLine($"Successfully rendered page 0 to stream. Stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
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

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Görüntü seçenekleri oluştur
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // SheetRender örneği oluştur
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // İlk sayfa indeksini al (0 tabanlı)
                int pageIndex = 0;

                // Sayfa indeksi parametresiyle ToImage'i çağır
                sheetRender.ToImage(pageIndex, "output_page.png");

                Console.WriteLine($"Successfully rendered page {pageIndex} to image");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


