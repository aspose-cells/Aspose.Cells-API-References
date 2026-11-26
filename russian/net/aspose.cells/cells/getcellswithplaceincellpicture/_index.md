---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает все ячейки, содержащие встроенное изображение"
type: docs
url: /ru/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Получает все ячейки, содержащие встроенное изображение.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Возвращаемое значение

Перечислитель для перебора всех объектов Cell, содержащих встроенное изображение

### Примечания

Если в этом листе нет изображения, установленного как "Place in Cell", будет возвращено null.

### Примеры

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить изображение на лист (это не будет учитываться методом GetCellsWithPlaceInCellPicture)
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // Добавить встроенное изображение в ячейку B3 (это будет учитываться)
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // Удалить плавающее изображение
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // Получить ячейки со встроенными изображениями
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // Сохранить и перезагрузить, чтобы проверить сохранность
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // Проверить после перезагрузки
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


