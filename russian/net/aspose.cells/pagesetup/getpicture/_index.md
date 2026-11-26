---
title: "PageSetup.GetPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Получает объект Picture заголовка/нижнего колонтитула"
type: docs
url: /ru/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Получает объект [`Picture`](../../../aspose.cells.drawing/picture/) заголовка/нижнего колонтитула.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isHeader | Boolean | Указывает, находится ли он в заголовке или нижнем колонтитуле. |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

### Возвращаемое значение

Возвращает объект [`Picture`](../../../aspose.cells.drawing/picture/). Возвращает null, если изображение отсутствует.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте изображение в заголовок листа
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // Получите изображение из заголовка и измените его яркость
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Получает объект [`Picture`](../../../aspose.cells.drawing/picture/) заголовка/нижнего колонтитула.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isFirst | Boolean | Указывает, получаем ли изображение из заголовка/нижнего колонтитула первой страницы. |
| isEven | Boolean | Указывает, получаем ли изображение из заголовка/нижнего колонтитула чётной страницы. |
| isHeader | Boolean | Указывает, получаем ли изображение из заголовка/нижнего колонтитула. |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |

### Возвращаемое значение

Возвращает объект [`Picture`](../../../aspose.cells.drawing/picture/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить объект PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Установите некоторые свойства заголовка/нижнего колонтитула, чтобы убедиться, что есть изображения для получения.
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // Вызовите метод GetPicture с параметрами: isFirst, isEven, isHeader, section
                // Проверка заголовка первой страницы (раздел 0 — центрированный заголовок)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // Сохраните книгу
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


