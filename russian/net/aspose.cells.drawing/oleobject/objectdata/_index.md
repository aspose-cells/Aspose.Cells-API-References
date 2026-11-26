---
title: "OleObject.ObjectData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Представляет данные встроенного OLE‑объекта в виде массива байтов"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Представляет данные вложенного ole‑объекта в виде массива байтов.

```csharp
public byte[] ObjectData { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            var workbook = new Workbook();
            
            // Получить доступ к первому листу
            var worksheet = workbook.Worksheets[0];
            
            // Пример путей к файлам (замените их фактическими путями в вашей среде)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // Добавить OLE‑объект с начальными данными изображения
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // Изменить данные OLE‑объекта
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // Сохраните книгу
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


