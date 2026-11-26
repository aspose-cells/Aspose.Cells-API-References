---
title: "ShapeCollection.AddFreeFloatingShape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет свободно плавающую форму на лист. Применяется только к линиям/изображениям"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addfreefloatingshape/
---
## ShapeCollection.AddFreeFloatingShape method

Добавляет свободно плавающую форму на лист. Применяется только к форме линии/изображения.

```csharp
public Shape AddFreeFloatingShape(MsoDrawingType type, int top, int left, int height, int width, 
    byte[] imageData, bool isOriginalSize)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | MsoDrawingType | Тип формы. |
| верх | Int32 | Представляет вертикальное смещение формы от верхней строки листа, в пикселях. |
| влево | Int32 | Представляет горизонтальное смещение формы от левого столбца листа, в пикселях. |
| высота | Int32 | Представляет высоту LineShape, в пикселях. |
| ширина | Int32 | Представляет ширину LineShape, в пикселях. |
| imageData | Byte[] | Данные изображения, применяются только к картинке. |
| isOriginalSize | Boolean | Определяет, использует ли форма оригинальный размер, если форма является изображением. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeFloatingShapeWithMsoDrawingTypeInt32Int32Int32IDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Добавьте линейную фигуру
            Shape floatingShape_Line = shapes.AddFreeFloatingShape(
                MsoDrawingType.Line, 
                100, 100, 100, 50, 
                null, 
                false);

            // Добавьте форму изображения (используя пример данных изображения)
            byte[] imageData = null;
            try
            {
                using (FileStream fs = new FileStream("image.jpg", FileMode.Open))
                {
                    imageData = new byte[fs.Length];
                    fs.Read(imageData, 0, (int)fs.Length);
                }
            }
            catch
            {
                // Создайте фиктивные данные изображения, если файл не найден
                imageData = new byte[100];
            }

            Shape floatingShape_Picture = shapes.AddFreeFloatingShape(
                MsoDrawingType.Picture, 
                200, 100, 100, 50, 
                imageData, 
                false);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


