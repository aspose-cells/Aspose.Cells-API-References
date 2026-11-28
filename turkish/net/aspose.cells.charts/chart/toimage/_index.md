---
title: "Chart.ToImage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart yöntemi. Grafiğin 32 bit Bitmap nesnesini alır"
type: docs
url: /tr/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Grafiğin 32-bit `Bitmap` nesnesini alır.

```csharp
public Bitmap ToImage()
```

### Dönüş Değeri

grafiğin resmi.

### Açıklamalar

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, null dönecektir.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // Bir sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);
            
            // Grafiği görüntüye dönüştür ve dosyaya kaydet
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Grafiğin 32-bit `Bitmap` nesnesini alır. `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression ve ImageOrPrintOptions.Quality öznitelikleri göz ardı edilir.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri |

### Dönüş Değeri

grafiğin resmi.

### Açıklamalar

32 bitlik bir bitmap nesnesi döndürür, bu nedenle ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression ve ImageOrPrintOptions.Quality özellikleri yöntemi etkilemez. Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, null dönecektir.

### Örnekler

200 x dpi ve 300 y dpi değerlerine sahip bir bitmap nesnesi alır.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 200;
options.VerticalResolution = 300;

Workbook book = new Workbook(@"test.xls");
Bitmap chartObject = book.Worksheets[0].Charts[0].ToImage(options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 200
options.VerticalResolution = 300

Dim book As Workbook =  New Workbook("test.xls")
Dim chartObject As Bitmap = book.Worksheets(0).Charts(0).ToImage(options)

```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler.

```csharp
public void ToImage(string imageFile)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | String | Tam yol içeren görüntü dosya adı. |

### Açıklamalar

Görüntünün formatı, dosya adının uzantısı kullanılarak belirtilir. Örneğin, "myfile.png" belirlerseniz, görüntü PNG formatında kaydedilir. Aşağıdaki dosya uzantıları tanınır: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Grafiği görüntü olarak kaydet
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

Grafik görüntüsünü oluşturur ve belirtilen formatta bir dosyaya kaydeder.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | String | Tam yol içeren görüntü dosya adı. |
| imageFormat | ImageFormat | Görüntünün kaydedileceği format. |

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Chart.ToImage(string, ImageType) yöntemini kullanın. Bu özellik Temmuz 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Grafik görüntüsünü oluşturur ve belirtilen görüntü türünde bir dosyaya kaydeder.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | String | Tam yol içeren görüntü dosya adı. |
| imageType | ImageType | Görüntünün kaydedileceği görüntü türü. |

### Açıklamalar

Görüntünün türü `imageType` kullanılarak belirtilir. Aşağıdaki türler desteklenir: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Grafiği belirtilen ImageType ile görüntüye kaydet
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Grafik görüntüsünü oluşturur ve Jpeg formatında bir dosyaya kaydeder.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | String | Tam yol içeren görüntü dosya adı. |
| jpegQuality | Int64 | Jpeg kalitesi. |

### Açıklamalar

Genişlik veya yükseklik sıfır ise ya da grafik Supported Charts List'e göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, belirtilen kaliteyle ToImage(string,ImageOrPrintOptions) yöntemini kullanın. Bu yöntem Mart 2025'ten itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodToImageWithStringInt64Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // ToImage yöntemini (String, Int64) parametreleriyle çağırın.
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Grafik görüntüsünü oluşturur ve Jpeg formatında bir akışa kaydeder.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Çıktı akışı. |
| jpegQuality | Int64 | Jpeg kalitesi. |

### Açıklamalar

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamInt64Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Görüntüyü kaydetmek için bir bellek akışı oluştur
                using (MemoryStream stream = new MemoryStream())
                {
                    // ToImage yöntemini Stream ve Int64 parametreleriyle çağırın.
                    // JPEG kalitesi 80 olarak belirtilir (geçerli aralık genellikle 0-100'dür).
                    chart.ToImage(stream, 80);

                    // Başarı mesajını göster
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Çalışma kitabını kaydedin
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Çıktı akışı. |
| imageFormat | ImageFormat | Görüntünün kaydedileceği format. |

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, Chart.ToImage(Stream, ImageType) yöntemini kullanın. Bu özellik Temmuz 2022'den itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Görüntüyü kaydetmek için bir bellek akışı oluştur
                using (MemoryStream stream = new MemoryStream())
                {
                    // ToImage yöntemini Stream ve ImageFormat parametreleriyle çağırın.
                    // System.Drawing.Imaging.ImageFormat yerine Aspose.Cells.Drawing.ImageType kullanarak
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // Başarı mesajını göster
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // İsteğe bağlı olarak akışı doğrulama için bir dosyaya kaydedin.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ToImage: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Çıktı akışı. |
| imageType | ImageType | Görüntünün kaydedileceği görüntü türü. |

### Açıklamalar

Görüntünün türü `imageType` kullanılarak belirtilir. Aşağıdaki türler desteklenir: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Genişlik veya yükseklik sıfır ise ya da grafik Desteklenen Grafikler Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Görüntüyü kaydetmek için bir bellek akışı oluştur
                using (MemoryStream stream = new MemoryStream())
                {
                    // ToImage yöntemini Stream ve ImageType parametreleriyle çağırın.
                    chart.ToImage(stream, ImageType.Png);

                    // Başarı mesajını göster
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // Görseli gösterim amacıyla bir dosyaya kaydedin.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ChartToImageDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün formatını belirler.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| imageFile | String | Tam yol içeren görüntü dosya adı. |
| seçenekler | ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri |

### Açıklamalar

Görüntünün formatı, dosya adının uzantısı kullanılarak belirtilir. Örneğin, "myfile.png" belirlerseniz, görüntü PNG formatında kaydedilir. Aşağıdaki dosya uzantıları tanınır: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Genişlik veya yükseklik sıfır ise ya da grafik Supported Charts List'e göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Daha fazla ayrıntı için lütfen [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) adresine bakın.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodToImageWithStringImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Görüntü seçenekleri oluştur
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // Çalışma kitabını yükle
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

            // Grafiği görüntüye kaydet
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Grafik görüntüsünü oluşturur ve belirtilen formatta bir akışa kaydeder.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Çıktı akışı. |
| seçenekler | ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri |

### Açıklamalar

Görüntünün türü `options.ImageType` kullanılarak belirtilir. Aşağıdaki formatlar desteklenir: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Genişlik veya yükseklik sıfır ise ya da grafik Supported Charts List'e göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Daha fazla ayrıntı için lütfen [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) adresine bakın.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ChartMethodToImageWithStreamImageOrPrintOptDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Görüntüyü kaydetmek için bir bellek akışı oluştur
                using (MemoryStream stream = new MemoryStream())
                {
                    // Belirli ayarlarla ImageOrPrintOptions oluşturun
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // ToImage yöntemini Stream ve ImageOrPrintOptions parametreleriyle çağırın.
                    chart.ToImage(stream, options);

                    // Başarı mesajını göster
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Çalışma kitabını kaydedin
                    workbook.Save("ChartToImageDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error converting chart to image: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


