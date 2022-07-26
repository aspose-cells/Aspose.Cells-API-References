---
title: ToImage
second_title: Справочник по Aspose.Cells для .NET API
description: Получает 32-битныйБитовая карта объект диаграммы.
type: docs
weight: 590
url: /ru/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Получает 32-битный`Битовая карта` объект диаграммы.

```csharp
public Bitmap ToImage()
```

### Возвращаемое значение

картинка графика.

### Примечания

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, будет возвращено значение null. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Смотрите также

* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Получает 32-битный`Битовая карта` объект диаграммы. `ImageOrPrintOptions.ImageFormat` , атрибуты ImageOrPrintOptions.TiffCompression и ImageOrPrintOptions.Quality игнорируются.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| options | ImageOrPrintOptions | Дополнительные возможности создания образа |

### Возвращаемое значение

картинка графика.

### Примечания

Возвращает 32-битный растровый объект, поэтому атрибуты ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression и ImageOrPrintOptions.Quality не влияют на метод. вернет null. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Примеры

Получает растровый объект с разрешением 200 x dpi и 300 y dpi.

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

### Смотрите также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Создает изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения.

```csharp
public void ToImage(string imageFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путем. |

### Примечания

Формат изображения задается расширением имени файла. Например, если указать "myfile.png", то изображение будет сохранено в формате PNG. Распознаются следующие расширения файлов: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, этот метод ничего не даст. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Смотрите также

* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Создает изображение диаграммы и сохраняет его в файл с указанным типом изображения.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путем. |
| imageType | ImageType | Тип изображения, в котором нужно сохранить изображение. |

### Примечания

Тип изображения указывается с помощью`Тип изображения`. Поддерживаются следующие типы: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, этот метод ничего не даст. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Смотрите также

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Создает изображение графика и сохраняет его в файл в формате Jpeg.

```csharp
public void ToImage(string imageFile, long jpegQuality)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путем. |
| jpegQuality | Int64 | Качество JPEG. |

### Примечания

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, этот метод ничего не даст. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Смотрите также

* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Создает изображение диаграммы и сохраняет его в поток в формате Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Выходной поток. |
| jpegQuality | Int64 | Качество JPEG. |

### Примечания

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, этот метод ничего не даст. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Смотрите также

* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Создает изображение диаграммы и сохраняет его в потоке в указанном формате.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Выходной поток. |
| imageType | ImageType | Тип изображения, в котором нужно сохранить изображение. |

### Примечания

Тип изображения указывается с помощью`Тип изображения`. Поддерживаются следующие типы: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, этот метод ничего не даст. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Смотрите также

* enum [ImageType](../../../aspose.cells.drawing/imagetype)
* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Создает изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путем. |
| options | ImageOrPrintOptions | Дополнительные возможности создания образа |

### Примечания

Формат изображения задается расширением имени файла. Например, если указать "myfile.png", то изображение будет сохранено в формате PNG. Распознаются следующие расширения файлов: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, этот метод ничего не даст. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Примеры

Сохраняет в формате Tiff с разрешением 300 dpi и сжатием CCITT4. Сохраняет в формате Jpeg с разрешением 300 dpi и качеством изображения 80.

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

### Смотрите также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Создает изображение диаграммы и сохраняет его в потоке в указанном формате.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Выходной поток. |
| options | ImageOrPrintOptions | Дополнительные возможности создания образа |

### Примечания

Тип изображения указывается с помощью`options.ImageType`. Поддерживаются следующие форматы: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Если ширина или высота равны нулю или диаграмма не поддерживается в соответствии со списком поддерживаемых диаграмм, этот метод ничего не даст. См.[Список поддерживаемых диаграмм](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для более подробной информации.

### Смотрите также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions)
* class [Chart](../../chart)
* пространство имен [Aspose.Cells.Charts](../../chart)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
