---
title: "Worksheet.ErrorCheckOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает настройки проверки ошибок, применяемые к определённым диапазонам"
type: docs
url: /ru/net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Получает настройки проверки ошибок, применяемые к определённым диапазонам.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyErrorCheckOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Включите параметры проверки ошибок
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            ErrorCheckOption option = options[0]; // Properly access first option using indexer
            option.SetErrorCheck(ErrorCheckType.TextDate, true);
            option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
            
            // Получите количество диапазонов для этой опции
            int rangeCount = option.GetCountOfRange();
            Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
            
            // Сохраните книгу
            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### См. также

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


