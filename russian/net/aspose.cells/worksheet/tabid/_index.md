---
title: "Worksheet.TabId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet property. Указывает внутренний идентификатор листа"
type: docs
url: /ru/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Указывает внутренний идентификатор листа.

```csharp
public int TabId { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить свойство TabId
            worksheet.TabId = 107;
            
            // Сохраните книгу
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // Загрузить сохранённую книгу, чтобы проверить TabId
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Отобразить значение TabId
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


