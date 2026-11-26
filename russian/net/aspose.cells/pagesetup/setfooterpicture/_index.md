---
title: "PageSetup.SetFooterPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PageSetup. Устанавливает изображение в нижний колонтитул листа"
type: docs
url: /ru/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

Устанавливает изображение в нижний колонтитул листа.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| секция | Int32 | 0: Левая секция, 1: Центральная секция, 2: Правая секция. |
| footerPicture | Byte[] | Данные изображения. |

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

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Загрузить файл изображения в массив байтов
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // Вызовите метод SetFooterPicture с индексом секции (0 — центр, 1 — слева, 2 — справа) и данными изображения
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // Установите текст нижнего колонтитула, отображаемый вместе с изображением
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // Сохраните книгу, чтобы увидеть изображение нижнего колонтитула
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
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


