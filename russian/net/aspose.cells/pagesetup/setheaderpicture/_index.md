---
title: "PageSetup.SetHeaderPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает изображение в заголовке листа"
type: docs
url: /ru/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

Устанавливает изображение в верхний колонтитул листа.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| headerPicture | Byte[] | Данные изображения. |

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

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Загрузить файл изображения в массив байтов
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // Вызвать SetHeaderPicture с индексом секции (0 для центрального заголовка) и байтами изображения
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // Установить скрипт заголовка для отображения изображения
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // Сохраните книгу
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### См. также

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


