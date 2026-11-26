---
title: "Worksheet.FirstVisibleRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Представляет индекс первой видимой строки"
type: docs
url: /ru/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Представляет индекс первой видимой строки.

```csharp
public int FirstVisibleRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите некоторые примерные данные
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Установить первую видимую строку на строку 20
            worksheet.FirstVisibleRow = 20;
            
            // Отобразить первую видимую строку
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // Сохраните книгу
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


