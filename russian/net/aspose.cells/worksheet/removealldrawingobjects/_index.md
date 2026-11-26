---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet method. Удаляет все графические объекты на этом листе"
type: docs
url: /ru/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Удаляет все графические объекты в этом листе.

```csharp
public void RemoveAllDrawingObjects()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить несколько графических объектов на лист
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // Сохранить перед удалением объектов
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // Удалить все графические объекты
            worksheet.RemoveAllDrawingObjects();
            
            // Сохранить после удаления объектов
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // Освободить ресурсы книги
            workbook.Dispose();
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


