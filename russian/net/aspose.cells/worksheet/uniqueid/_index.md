---
title: "Worksheet.UniqueId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает и задает уникальный идентификатор, он совпадает с 15DB5C3CA5A148AF8F253D86AC232D4F"
type: docs
url: /ru/net/aspose.cells/worksheet/uniqueid/
---
## Worksheet.UniqueId property

Получает и задает уникальный идентификатор, он совпадает с {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F}.

```csharp
public string UniqueId { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyUniqueIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Сгенерировать уникальный идентификатор для листа
            string uniqueId = "{" + Guid.NewGuid().ToString() + "}";
            
            // Установить свойство UniqueId первого листа
            workbook.Worksheets[0].UniqueId = uniqueId;
            
            // Сохраните книгу
            string outputPath = "SheetUniqueIdDemo.xlsx";
            workbook.Save(outputPath);
            
            // Перезагрузить книгу, чтобы проверить, сохраняется ли UniqueId
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Вывести UniqueId для демонстрации функциональности
            Console.WriteLine("Worksheet UniqueId: " + loadedWorkbook.Worksheets[0].UniqueId);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


