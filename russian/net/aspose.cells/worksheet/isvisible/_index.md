---
title: "Worksheet.IsVisible"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet property. Представляет, видим ли лист"
type: docs
url: /ru/net/aspose.cells/worksheet/isvisible/
---
## Worksheet.IsVisible property

Представляет, видим ли лист.

```csharp
public bool IsVisible { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте 3 листа
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Сделайте второй лист скрытым
            workbook.Worksheets[1].IsVisible = false;
            
            // Сохраните книгу
            workbook.Save("WorksheetVisibilityDemo.xlsx");
            
            // Отобразить статус видимости
            Console.WriteLine("Worksheet Visibility Status:");
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Console.WriteLine($"{workbook.Worksheets[i].Name}: {(workbook.Worksheets[i].IsVisible ? "Visible" : "Hidden")}");
            }
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


