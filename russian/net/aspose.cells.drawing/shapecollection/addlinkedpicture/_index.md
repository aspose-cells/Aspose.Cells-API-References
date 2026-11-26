---
title: "ShapeCollection.AddLinkedPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавить связанную картинку"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addlinkedpicture/
---
## ShapeCollection.AddLinkedPicture method

Добавить связанную картинку.

```csharp
public Picture AddLinkedPicture(int topRow, int leftColumn, int height, int width, 
    string sourceFullName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| высота | Int32 | Высота фигуры. В пикселях |
| ширина | Int32 | Ширина фигуры. В пикселях |
| sourceFullName | String | Путь и имя исходного файла для связанного изображения |

### Возвращаемое значение

[`Picture`](../../picture/) Picture object.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLinkedPictureWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерный текст в ячейку A1
            worksheet.Cells["A1"].PutValue("Image will be linked below:");
            
            // Добавить связанную картинку в лист
            string imageUrl = "https://example.com/sample.jpg";
            worksheet.Shapes.AddLinkedPicture(1, 1, 100, 100, imageUrl);
            
            // Сохраните книгу
            workbook.Save("output_with_linked_picture.xlsx");
            
            Console.WriteLine("Workbook saved with linked picture.");
        }
    }
}
```

### См. также

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


