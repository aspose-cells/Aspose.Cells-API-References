---
title: "Worksheet.TransitionEntry"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, включена ли опция совместимости Lotus для Transition Formula Entry"
type: docs
url: /ru/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Указывает, включена ли опция Transition Formula Entry (совместимость с Lotus).

```csharp
public bool TransitionEntry { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить свойство TransitionEntry
            worksheet.TransitionEntry = true;
            
            // Отобразить значение TransitionEntry
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузить сохранённую книгу, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Отобразить загруженное значение TransitionEntry
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


