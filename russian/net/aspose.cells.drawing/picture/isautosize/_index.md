---
title: "Picture.IsAutoSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Picture. True указывает, что размер ole‑объекта будет автоматически изменён в соответствии с размером снимка встроенного содержимого при активации ole‑объекта"
type: docs
url: /ru/net/aspose.cells.drawing/picture/isautosize/
---
## Picture.IsAutoSize property

True указывает, что размер OLE‑объекта будет автоматически изменён до размера снимка встроенного содержимого при активации OLE‑объекта.

```csharp
public bool IsAutoSize { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить изображение на лист
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Продемонстрировать свойство IsAutoSize
            Console.WriteLine("Original IsAutoSize value: " + picture.IsAutoSize);
            
            // Установить IsAutoSize в true — изображение будет автоматически изменять размер, чтобы соответствовать содержимому
            picture.IsAutoSize = true;
            Console.WriteLine("After setting IsAutoSize to true: " + picture.IsAutoSize);
            
            // Установить IsAutoSize в false — изображение сохранит свои исходные размеры
            picture.IsAutoSize = false;
            Console.WriteLine("After setting IsAutoSize to false: " + picture.IsAutoSize);

            // Сохраните книгу
            workbook.Save("PicturePropertyIsAutoSizeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


