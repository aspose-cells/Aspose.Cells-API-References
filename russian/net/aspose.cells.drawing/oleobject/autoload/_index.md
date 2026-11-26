---
title: "OleObject.AutoLoad"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство OleObject. Указывает, будет ли вызываемое хост-приложение для встроенного объекта загружать данные объекта автоматически при открытии родительской книги."
type: docs
url: /ru/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Указывает, будет ли вызываемое хост‑приложение для встроенного объекта загружать данные объекта автоматически при открытии родительской книги.

```csharp
public bool AutoLoad { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить OleObject в worksheet
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // Установить свойства OleObject
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // Продемонстрировать свойство AutoLoad
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // Сохраните книгу
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### См. также

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


