---
title: "OleObject.ClassIdentifier"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Получает и задаёт идентификатор класса встроенного объекта. Он определяет, какое приложение открывает встроенный файл"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

Получает и задает идентификатор класса встроенного объекта. Это определяет, какое приложение открывает встроенный файл.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyClassIdentifierDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Пример массива байтов для ClassIdentifier (обычно это будет реальный идентификатор класса)
            byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 
                                         0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };

            // Добавить OLE‑объект с примерными данными
            int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
            OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Задать свойство ClassIdentifier
            oleObject.ClassIdentifier = classId;
            oleObject.ProgID = "Excel.Sheet.12";
            oleObject.DisplayAsIcon = true;

            // Сохраните книгу
            workbook.Save("OleObjectDemo.xlsx");

            // Загрузить сохранённую книгу, чтобы проверить ClassIdentifier
            Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
            OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
            
            // Проверьте, что ClassIdentifier сохранён
            Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


