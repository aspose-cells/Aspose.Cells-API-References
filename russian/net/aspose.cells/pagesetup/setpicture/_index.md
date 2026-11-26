---
title: "PageSetup.SetPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает изображение в верхний/нижний колонтитул листа"
type: docs
url: /ru/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

Устанавливает изображение в верхний/нижний колонтитул листа.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isFirst | Boolean | Указывает, устанавливается ли изображение в верхний/нижний колонтитул первой страницы. |
| isEven | Boolean | Указывает, устанавливается ли изображение в верхний/нижний колонтитул чётной страницы. |
| isHeader | Boolean | Указывает, устанавливается ли изображение в верхний/нижний колонтитул. |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| imageData | Byte[] | Данные изображения. |

### Возвращаемое значение

Возвращает объект [`Picture`](../../../aspose.cells.drawing/picture/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Загрузить файл изображения в массив байтов
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // Вызвать метод SetPicture, чтобы установить изображение заголовка
                // Параметры: isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // Установить текст заголовка
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // Сохраните книгу
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
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


