---
title: "OleObject.ImageData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Представляет изображение OLE‑объекта в виде массива байтов"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/imagedata/
---
## OleObject.ImageData property

Представляет изображение ole‑объекта в виде массива байтов.

```csharp
public byte[] ImageData { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyImageDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Прочитать файл изображения в массив байтов
            byte[] imageBytes = File.ReadAllBytes("image1.png");
            
            // Добавить OLE‑объект с данными изображения
            int oleIndex = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, imageBytes);
            OleObject oleObject = workbook.Worksheets[0].OleObjects[oleIndex];
            
            // Установить свойства встроенного объекта
            oleObject.SetEmbeddedObject(false, imageBytes, "image1.png", true, "Sample Image", false);
            
            // Продемонстрировать использование свойства ImageData
            Console.WriteLine($"Image data length: {oleObject.ImageData.Length}");
            Console.WriteLine($"First byte: {oleObject.ImageData[0]}");
            Console.WriteLine($"Middle byte: {oleObject.ImageData[oleObject.ImageData.Length/2]}");
            Console.WriteLine($"Last byte: {oleObject.ImageData[oleObject.ImageData.Length-1]}");
            
            // Сохраните книгу
            workbook.Save("OleObjectWithImage.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


