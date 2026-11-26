---
title: "PictureCollection.Camera"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PictureCollection. Делает снимок диапазона"
type: docs
url: /ru/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Снимает фотографию диапазона.

```csharp
public int Camera(int row, int column, string range)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки этого изображения. |
| column | Int32 | Индекс столбца этого изображения. |
| диапазон | String | Область, требующая фотосъёмки |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые примерные данные, чтобы создать диапазон
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Получите коллекцию Pictures из листа
                PictureCollection pictures = worksheet.Pictures;

                // Вызовите метод Camera, чтобы создать изображение камеры
                // Параметры: row (строка в левом верхнем углу), column (столбец в левом верхнем углу), range (исходный диапазон)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Сохраните книгу
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


