---
title: "ErrorCheckOption.AddRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ErrorCheckOption. Добавляет один диапазон, влияющий на эту настройку"
type: docs
url: /ru/net/aspose.cells/errorcheckoption/addrange/
---
## ErrorCheckOption.AddRange method

Добавляет один затронутый диапазон этим параметром.

```csharp
public int AddRange(CellArea ca)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ca | CellArea | Диапазон, который будет добавлен. |

### Возвращаемое значение

Индекс добавленного диапазона в списке диапазонов этой настройки.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodAddRangeWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;
            int index = optsCollection.Add();
            ErrorCheckOption opts = optsCollection[index];
            
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            
            // Добавить диапазоны с помощью CellArea
            opts.AddRange(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 3 }); // A1:D2
            opts.AddRange(new CellArea { StartRow = 2, StartColumn = 0, EndRow = 2, EndColumn = 3 }); // A3:D3
            
            // Сохраните книгу
            workbook.Save("ErrorCheckOptionMethodAddRangeWithCellAreaDemo.xls");
            
            Console.WriteLine("Workbook saved with error check options.");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


