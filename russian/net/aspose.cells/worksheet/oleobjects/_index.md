---
title: "Worksheet.OleObjects"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Представляет коллекцию OleObject в листе"
type: docs
url: /ru/net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

Представляет коллекцию [`OleObject`](../../../aspose.cells.drawing/oleobject/) в листе.

```csharp
public OleObjectCollection OleObjects { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOleObjectsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить OleObject в worksheet
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
            OleObject ole = worksheet.OleObjects[oleObjectIndex];
            
            // Изменить свойства OleObject
            ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
            ole.FileFormatType = FileFormatType.Xlsx;

            // Сохраните книгу
            workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


