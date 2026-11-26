---
title: "Chart.ToImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Chart. Получает 32‑битный объект Bitmap диаграммы"
type: docs
url: /ru/net/aspose.cells.charts/chart/toimage/
---
## ToImage() {#toimage}

Получает 32‑битный объект `Bitmap` диаграммы.

```csharp
public Bitmap ToImage()
```

### Возвращаемое значение

изображение диаграммы.

### Примечания

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, будет возвращено null.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["B4"].PutValue(1500);

            // Добавить столбчатую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);
            
            // Преобразовать диаграмму в изображение и сохранить в файл
            chart.ToImage("ChartImage.png", ImageType.Png);
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(ImageOrPrintOptions) {#toimage_1}

Получает 32‑битный объект `Bitmap` диаграммы. Атрибуты `ImageOrPrintOptions.ImageFormat`, ImageOrPrintOptions.TiffCompression и ImageOrPrintOptions.Quality игнорируются.

```csharp
public Bitmap ToImage(ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | ImageOrPrintOptions | Дополнительные параметры создания изображения |

### Возвращаемое значение

изображение диаграммы.

### Примечания

Возвращает 32‑битный объект bitmap, поэтому атрибуты ImageOrPrintOptions.ImageFormat, ImageOrPrintOptions.TiffCompression и ImageOrPrintOptions.Quality не влияют на метод. Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, будет возвращено null.

### Примеры

Получает объект bitmap с разрешением 200 dpi по оси x и 300 dpi по оси y.

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

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_6}

Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения.

```csharp
public void ToImage(string imageFile)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путём. |

### Примечания

Формат изображения задаётся с помощью расширения имени файла. Например, если указать "myfile.png", изображение будет сохранено в формате PNG. Распознаются следующие расширения файлов: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(45);
            worksheet.Cells["B3"].PutValue(55);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Сохранить диаграмму как изображение
            chart.ToImage("ChartImage.jpg");
            
            Console.WriteLine("Chart saved as image successfully.");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageFormat) {#toimage_10}

Создаёт изображение диаграммы и сохраняет его в файл в указанном формате.

```csharp
[Obsolete("Use Chart.ToImage(string, ImageType) method instead.")]
public void ToImage(string imageFile, ImageFormat imageFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путём. |
| imageFormat | ImageFormat | Формат, в котором сохранять изображение. |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Chart.ToImage(string, ImageType). Это свойство будет удалено через 12 месяцев, начиная с июля 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageType) {#toimage_7}

Создаёт изображение диаграммы и сохраняет его в файл в указанном типе изображения.

```csharp
public void ToImage(string imageFile, ImageType imageType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путём. |
| imageType | ImageType | Тип изображения, в котором сохранять файл. |

### Примечания

Тип изображения задаётся с помощью `imageType`. Поддерживаются следующие типы: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(7);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Сохранить диаграмму в изображение с указанным ImageType
            chart.ToImage("output_chart.png", ImageType.Png);

            Console.WriteLine("Chart saved to image successfully.");
        }
    }
}
```

### См. также

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, long) {#toimage_9}

Создает изображение диаграммы и сохраняет его в файл в формате Jpeg.

```csharp
[Obsolete("Use Chart.ToImage(string,ImageOrPrintOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ToImage(string imageFile, long jpegQuality)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путём. |
| jpegQuality | Int64 | Качество Jpeg. |

### Примечания

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает. ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод ToImage(string,ImageOrPrintOptions) с указанным качеством. Этот метод будет удалён через 12 месяцев, начиная с марта 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);
            
            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            try
            {
                // Вызовите метод ToImage с параметрами (String, Int64)
                string imagePath = "ChartImage.jpg";
                long jpegQuality = 90; // Quality percentage (0-100)
                chart.ToImage(imagePath, jpegQuality);
                
                Console.WriteLine($"Chart saved as image successfully to: {imagePath}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ToImage method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("ChartToImageDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, long) {#toimage_4}

Создаёт изображение диаграммы и сохраняет его в поток в формате Jpeg.

```csharp
public void ToImage(Stream stream, long jpegQuality)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Выходной поток. |
| jpegQuality | Int64 | Качество Jpeg. |

### Примечания

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Создать поток памяти для сохранения изображения
                using (MemoryStream stream = new MemoryStream())
                {
                    // Вызовите метод ToImage с параметрами Stream и Int64.
                    // Качество JPEG задаётся как 80 (допустимый диапазон обычно 0‑100).
                    chart.ToImage(stream, 80);

                    // Отобразить сообщение об успехе
                    Console.WriteLine("Chart successfully converted to image with JPEG quality 80");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Сохраните книгу
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

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageFormat) {#toimage_5}

Создаёт изображение диаграммы и сохраняет его в поток в указанном формате.

```csharp
[Obsolete("Use Chart.ToImage(Stream, ImageType) method instead.")]
public void ToImage(Stream stream, ImageFormat imageFormat)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Выходной поток. |
| imageFormat | ImageFormat | Формат, в котором сохранять изображение. |

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Chart.ToImage(Stream, ImageType). Это свойство будет удалено через 12 месяцев, начиная с июля 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Создать поток памяти для сохранения изображения
                using (MemoryStream stream = new MemoryStream())
                {
                    // Вызовите метод ToImage с параметрами Stream и ImageFormat.
                    // Использование Aspose.Cells.Drawing.ImageType вместо System.Drawing.Imaging.ImageFormat.
                    chart.ToImage(stream, Aspose.Cells.Drawing.ImageType.Png);

                    // Отобразить сообщение об успехе
                    Console.WriteLine("Chart successfully saved to stream in PNG format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // При желании сохраните поток в файл для проверки.
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

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageType) {#toimage_2}

Создаёт изображение диаграммы и сохраняет его в поток в указанном формате.

```csharp
public void ToImage(Stream stream, ImageType imageType)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Выходной поток. |
| imageType | ImageType | Тип изображения, в котором сохранять файл. |

### Примечания

Тип изображения задаётся с помощью `imageType`. Поддерживаются следующие типы: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Создать поток памяти для сохранения изображения
                using (MemoryStream stream = new MemoryStream())
                {
                    // Вызовите метод ToImage с параметрами Stream и ImageType.
                    chart.ToImage(stream, ImageType.Png);

                    // Отобразить сообщение об успехе
                    Console.WriteLine("Chart successfully converted to image in PNG format");

                    // Сохраните изображение в файл для демонстрации.
                    File.WriteAllBytes("ChartImage.png", stream.ToArray());
                }

                // Сохраните книгу
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

### См. также

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string, ImageOrPrintOptions) {#toimage_8}

Создаёт изображение диаграммы и сохраняет его в файл. Расширение имени файла определяет формат изображения.

```csharp
public void ToImage(string imageFile, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| imageFile | String | Имя файла изображения с полным путём. |
| опции | ImageOrPrintOptions | Дополнительные параметры создания изображения |

### Примечания

Формат изображения задаётся с помощью расширения имени файла. Например, если указать "myfile.png", изображение будет сохранено в формате PNG. Распознаются следующие расширения файлов: .bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает. Пожалуйста, обратитесь к [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для получения более подробной информации.

### Примеры

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
            // Создать параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            options.TiffCompression = TiffCompression.CompressionCCITT4;

            // Загрузить книгу.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные и создайте диаграмму
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

            // Сохранить диаграмму в изображение.
            chart.ToImage("chart.tiff", options);
        }
    }
}
```

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(Stream, ImageOrPrintOptions) {#toimage_3}

Создаёт изображение диаграммы и сохраняет его в поток в указанном формате.

```csharp
public void ToImage(Stream stream, ImageOrPrintOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | Stream | Выходной поток. |
| опции | ImageOrPrintOptions | Дополнительные параметры создания изображения |

### Примечания

Тип изображения указывается с помощью `options.ImageType`. Поддерживаются следующие форматы: ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.

Если ширина или высота равны нулю или диаграмма не поддерживается согласно списку поддерживаемых диаграмм, этот метод ничего не сделает. Пожалуйста, обратитесь к [Supported Charts List](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) для получения более подробной информации.

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Добавить диаграмму в лист
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Создать поток памяти для сохранения изображения
                using (MemoryStream stream = new MemoryStream())
                {
                    // Создайте ImageOrPrintOptions с конкретными настройками.
                    ImageOrPrintOptions options = new ImageOrPrintOptions();
                    options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                    options.HorizontalResolution = 300;
                    options.VerticalResolution = 300;

                    // Вызовите метод ToImage с параметрами Stream и ImageOrPrintOptions.
                    chart.ToImage(stream, options);

                    // Отобразить сообщение об успехе
                    Console.WriteLine("Chart successfully converted to image with custom options");
                    Console.WriteLine($"Image stream length: {stream.Length} bytes");

                    // Сохраните книгу
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

### См. также

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


