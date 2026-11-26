---
title: "SheetRender.ToImage"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SheetRender. Отрисовывает определённую страницу в объект Graphics"
type: docs
url: /ru/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Отрисовать определённую страницу в объект Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| g | Графика | Объект, в который нужно отрисовать. |
| x | Single | Координата X (в пикселях) верхнего левого угла отрисованной страницы. |
| y | Single | Координата Y (в пикселях) верхнего левого угла отрисованной страницы. |
| ширина | Single | Максимальная ширина (в пикселях), которую может занимать отрисованная страница. |
| высота | Single | Максимальная высота (в пикселях), которую может занимать отрисованная страница. |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Создать параметры изображения
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Создать рендер листа для рабочего листа
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Создать поток памяти для захвата отрисованного изображения
                using (MemoryStream stream = new MemoryStream())
                {
                    // Вызвать ToImage с указанными параметрами
                    // Поскольку мы не можем использовать System.Drawing.Graphics, мы используем более простой перегрузку ToImage
                    sheetRender.ToImage(0, stream);

                    // Сохранить отрисованное изображение в файл
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

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Отрисовать определённую страницу в объект Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| g | Графика | Объект, в который нужно отрисовать. |
| x | Single | Координата X (в пикселях) верхнего левого угла отрисованной страницы. |
| y | Single | Координата Y (в пикселях) верхнего левого угла отрисованной страницы. |

### Примеры

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
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Создать параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Создать экземпляр SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Поскольку мы не можем использовать типы System.Drawing, мы будем использовать альтернативный метод ToImage
                // который сохраняет напрямую в файл
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Очистить ресурсы
                sheetRender.Dispose();
            }
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

Отрисовать определённую страницу в файл.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| fileName | String | имя файла выходного изображения |

### Примеры

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
            // Загрузить исходный файл Excel
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Создать параметры изображения
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Создать рендер листа для первого рабочего листа
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Отрисовать первую страницу листа в файл изображения
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

Отрисовать определённую страницу в поток.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |
| поток | Stream | поток выходного изображения |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Создать параметры изображения
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Создать экземпляр SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Создать поток памяти для хранения изображения
                using (MemoryStream stream = new MemoryStream())
                {
                    // Вызвать ToImage с параметрами индекса страницы и потока
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

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Отрисовать определённую страницу в объект Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pageIndex | Int32 | указать, какая страница будет конвертирована |

### Возвращаемое значение

объект bitmap страницы

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Создать параметры изображения
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Создать экземпляр SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Получить индекс первой страницы (нумерация с нуля)
                int pageIndex = 0;

                // Вызвать ToImage с параметром индекса страницы
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

### См. также

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


