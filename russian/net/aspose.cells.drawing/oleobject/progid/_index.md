---
title: "OleObject.ProgID"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Получает или задаёт ProgID OLE‑объекта"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Получает или задает ProgID OLE‑объекта.

```csharp
public string ProgID { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyProgIDDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить OLE‑объект в лист
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // Задать ProgID для OLE‑объекта
            ole.ProgID = "AcroExch.Document.DC";
            
            // Отобразить ProgID
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // Сохраните книгу
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


