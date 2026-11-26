---
title: "Worksheet.ActiveCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает или задает активную ячейку листа"
type: docs
url: /ru/net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Получает или задает активную ячейку в рабочем листе.

```csharp
public string ActiveCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyActiveCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите активную ячейку в B2
            worksheet.ActiveCell = "B2";
            
            // Вывести адрес активной ячейки
            Console.WriteLine("Active Cell: " + worksheet.ActiveCell);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузить сохранённую книгу, чтобы проверить активную ячейку
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("Loaded Active Cell: " + loadedWorkbook.Worksheets[0].ActiveCell);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


