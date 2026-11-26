---
title: "OleObject.ImageType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Возвращает формат изображения ole‑объекта"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/imagetype/
---
## OleObject.ImageType property

Получает формат изображения ole‑объекта.

```csharp
public ImageType ImageType { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить OLE‑объект в лист
            byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Отобразите текущий тип изображения OLE‑объекта
            Console.WriteLine("Current ImageType value: " + oleObject.ImageType);

            // Продемонстрируйте, как использовать свойство ImageType
            if (oleObject.ImageType == ImageType.Unknown)
            {
                Console.WriteLine("The OLE object's image format is not recognized.");
            }
            else if (oleObject.ImageType == ImageType.Emf)
            {
                Console.WriteLine("The OLE object uses EMF image format.");
            }
            else if (oleObject.ImageType == ImageType.Png)
            {
                Console.WriteLine("The OLE object uses PNG image format.");
            }

            // Сохраните книгу
            workbook.Save("OleObjectImageTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


