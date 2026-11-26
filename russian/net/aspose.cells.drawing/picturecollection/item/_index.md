---
title: "PictureCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PictureCollection. Возвращает элемент Picture по указанному индексу"
type: docs
url: /ru/net/aspose.cells.drawing/picturecollection/item/
---
## PictureCollection indexer

Получает элемент [`Picture`](../../picture/) по указанному индексу.

```csharp
public Picture this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить коллекцию изображений
            PictureCollection pictures = worksheet.Pictures;
            
            // Добавить изображение (замените "image.png" на реальный путь к изображению)
            int index = pictures.Add(1, 1, "image.png");
            
            // Получить доступ к изображению с помощью свойства Item
            Picture pic = pictures[index];
            
            // Продемонстрировать использование свойства Item
            Console.WriteLine($"Picture at index {index} has width: {pic.Width} and height: {pic.Height}");
            
            // Изменить свойства изображения
            pic.Height = 200;
            pic.Width = 300;
            
            // Сохраните книгу
            workbook.Save("PictureCollectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Picture](../../picture/)
* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


