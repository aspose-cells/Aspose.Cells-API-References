---
title: "Worksheet.IsOutlineShown"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, следует ли отображать контур"
type: docs
url: /ru/net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Указывает, показывать ли контур.

```csharp
public bool IsOutlineShown { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsOutlineShownDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите отображение контура
            worksheet.IsOutlineShown = true;
            Console.WriteLine("Outline shown: " + worksheet.IsOutlineShown);
            
            // Сохраните и перезагрузите, чтобы продемонстрировать сохранность
            string filePath = "IsOutlineShownDemo.xlsx";
            workbook.Save(filePath);
            
            Workbook loadedWorkbook = new Workbook(filePath);
            Console.WriteLine("Reloaded - Outline shown: " + loadedWorkbook.Worksheets[0].IsOutlineShown);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


