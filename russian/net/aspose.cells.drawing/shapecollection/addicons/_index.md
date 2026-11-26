---
title: "ShapeCollection.AddIcons"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет svg‑изображение"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addicons/
---
## ShapeCollection.AddIcons method

Добавляет SVG‑изображение.

```csharp
public Picture AddIcons(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageByteData, byte[] compatibleImageData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| верх | Int32 | Представляет вертикальное смещение фигуры от её левой строки, в пикселях. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| влево | Int32 | Горизонтальное смещение фигуры от её левого столбца, в пикселях. |
| высота | Int32 | Высота фигуры, в пикселях. |
| ширина | Int32 | Ширина фигуры, в пикселях. |
| imageByteData | Byte[] | Байт-данные изображения. |
| compatibleImageData | Byte[] | Преобразованные данные изображения из svg, совместимые с Excel 2016 или более ранними версиями. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddIconsWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Создайте пример файла значка (в реальном использовании вы бы использовали существующий файл)
            string iconPath = "icon.svg";
            File.WriteAllText(iconPath, "<svg xmlns='http://www.w3.org/2000/svg' width='100' height='100'><circle cx='50' cy='50' r='40' fill='red'/></svg>");

            // Добавьте значок в рабочий лист
            using (FileStream fs = new FileStream(iconPath, FileMode.Open))
            {
                int len = (int)fs.Length;
                byte[] imageData = new byte[len];
                fs.Read(imageData, 0, len);
                Picture picture = shapes.AddIcons(4, 0, 5, 0, -1, -1, imageData, null);
            }

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Очистка (необязательно)
            File.Delete(iconPath);
        }
    }
}
```

### См. также

* class [Picture](../../picture/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


