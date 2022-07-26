---
title: ToImage
second_title: Aspose.Cells for .NET API Referansı
description: 32-bit alırbit eşlem grafiğin nesnesi.
type: docs
weight: 590
url: /tr/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

32-bit alır`bit eşlem` grafiğin nesnesi.

```csharp
public Bitmap ToImage()
```

### Geri dönüş değeri

tablonun resmi.

### Notlar

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, null dönecektir. Lütfen bakın[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Ayrıca bakınız

* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

32 bit alır`bit eşlem` grafiğin nesnesi. `ImageOrPrintOptions.ImageFormat` , ImageOrPrintOptions.TiffCompression ve ImageOrPrintOptions.Quality nitelikleri yok sayılır.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| options | ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri |

### Geri dönüş değeri

tablonun resmi.

### Notlar

32 bitlik bir bitmap nesnesi döndürür, bu nedenle ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression ve ImageOrPrintOptions.Quality öznitelikleri yöntemi etkilemez. Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, null. döndürür. Lütfen bakın[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Örnekler

200 x dpi ve 300 y dpi ile bir bitmap nesnesi alır.

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

### Ayrıca bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün biçimini belirler.

```csharp
public void ToImage(string imageFile)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| imageFile | String | Tam yollu görüntü dosyası adı. |

### Notlar

Resmin formatı, dosya adının uzantısı kullanılarak belirlenir. Örneğin, "dosyam.png" belirtirseniz, resim PNG formatında kaydedilir. Aşağıdaki dosya uzantıları tanınır: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Lütfen bkz.[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Ayrıca bakınız

* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Grafik görüntüsünü oluşturur ve belirtilen görüntü türünde bir dosyaya kaydeder.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| imageFile | String | Tam yollu görüntü dosyası adı. |
| imageType | ImageType | Görüntünün kaydedileceği görüntü türü. |

### Notlar

Görüntünün türü kullanılarak belirtilir.`Resim türü`. Aşağıdaki türler desteklenir: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Lütfen bkz.[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Ayrıca bakınız

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Grafik görüntüsünü oluşturur ve Jpeg biçiminde bir dosyaya kaydeder.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| imageFile | String | Tam yollu görüntü dosyası adı. |
| jpegQuality | Int64 | JPEG kalitesi. |

### Notlar

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Lütfen bkz.[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Ayrıca bakınız

* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Grafik görüntüsünü oluşturur ve onu Jpeg biçiminde bir akışa kaydeder.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Çıkış akışı. |
| jpegQuality | Int64 | JPEG kalitesi. |

### Notlar

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Lütfen bkz.[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Ayrıca bakınız

* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Grafik görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Çıkış akışı. |
| imageType | ImageType | Görüntünün kaydedileceği görüntü türü. |

### Notlar

Görüntünün türü kullanılarak belirtilir.`Resim türü`. Aşağıdaki türler desteklenir: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Lütfen bakın[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Ayrıca bakınız

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder. Dosya adının uzantısı görüntünün biçimini belirler.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| imageFile | String | Tam yollu görüntü dosyası adı. |
| options | ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri |

### Notlar

Resmin formatı, dosya adının uzantısı kullanılarak belirlenir. Örneğin, "dosyam.png" belirtirseniz, resim PNG formatında kaydedilir. Aşağıdaki dosya uzantıları tanınır: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Lütfen bkz.[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Örnekler

300 dpi ve CCITT4 sıkıştırma ile Tiff'e kaydeder. 300 dpi ve 80 görüntü kalitesiyle Jpeg'e kaydeder.

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.TiffCompression = TiffCompression.CompressionCCITT4;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Tiff", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions() 
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.TiffCompression = TiffCompression.CompressionCCITT4

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Tiff", options)

```

```csharp

[C#]
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
options.Quality = 80;

Workbook book = new Workbook(@"test.xls");
book.Worksheets[0].Charts[0].ToImage(@"chart.Jpeg", options);

[VB]
Dim options As ImageOrPrintOptions =  New ImageOrPrintOptions()
options.HorizontalResolution = 300
options.VerticalResolution = 300
options.Quality = 80

Dim book As Workbook =  New Workbook("test.xls")
book.Worksheets(0).Charts(0).ToImage("chart.Jpeg", options)

```

### Ayrıca bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Grafik görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| stream | Stream | Çıkış akışı. |
| options | ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri |

### Notlar

Görüntünün türü kullanılarak belirtilir.`seçenekler.ImageType`. Aşağıdaki biçimler desteklenir: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Genişlik veya yükseklik sıfırsa veya grafik Desteklenen Grafikler Listesine göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz. Lütfen bkz.[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.

### Ayrıca bakınız

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* ad alanı [Aspose.Cells.Charts](../../chart)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
