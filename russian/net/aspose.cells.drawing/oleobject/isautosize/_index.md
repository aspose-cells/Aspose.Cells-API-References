---
title: "OleObject.IsAutoSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. True указывает, что размер OLE‑объекта будет автоматически изменён в соответствии с размером снимка встроенного содержимого при активации OLE‑объекта"
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

True указывает, что размер OLE‑объекта будет автоматически изменён до размера снимка встроенного содержимого при активации OLE‑объекта.

```csharp
public bool IsAutoSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить OLE‑объект (используя данные файла в виде массива байтов)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // Установить и продемонстрировать свойство IsAutoSize
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // Изменить свойство
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // Сохраните книгу
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


