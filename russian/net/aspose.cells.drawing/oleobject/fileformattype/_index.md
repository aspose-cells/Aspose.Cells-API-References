---
title: "OleObject.FileFormatType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Получает и задаёт тип файла встроенных данных ole‑объекта"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Получает и задает тип файла вложенных данных ole‑объекта

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте OLE‑объект в лист (без файловых данных)
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // Получите добавленный OLE‑объект
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // Установите и отобразите тип формата файла
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // Сохраните книгу
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


