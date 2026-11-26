---
title: "Worksheet.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает или задает имя листа"
type: docs
url: /ru/net/aspose.cells/worksheet/name/
---
## Worksheet.Name property

Получает или задаёт имя листа.

```csharp
public string Name { get; set; }
```

### Примечания

Максимальная длина имени листа составляет 31 символов. И вы не можете назначить одинаковое имя (без учёта регистра) двум листам. Например, вы не можете установить "SheetName1" для первого листа и установить "SHEETNAME1" для второго листа.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и задайте его имя
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Добавьте новый лист с определённым именем
            Worksheet newSheet = workbook.Worksheets.Add("ReportSheet");
            
            // Выведите имена всех листов
            Console.WriteLine("Worksheet Names:");
            foreach (Worksheet ws in workbook.Worksheets)
            {
                Console.WriteLine(ws.Name);
            }
            
            // Сохраните книгу
            workbook.Save("WorksheetNamesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


