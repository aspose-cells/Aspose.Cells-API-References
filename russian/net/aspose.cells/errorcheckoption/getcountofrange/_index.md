---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ErrorCheckOption. Возвращает количество диапазонов, влияющих на эту настройку"
type: docs
url: /ru/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Получает количество диапазонов, затронутых этим параметром.

```csharp
public int GetCountOfRange()
```

### Возвращаемое значение

Количество диапазонов, влияющих на эту настройку.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Получить коллекцию параметров проверки ошибок
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // Добавить первую опцию проверки ошибок
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // Добавить вторую опцию проверки ошибок
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // Продемонстрировать метод GetCountOfRange
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // Сохраните книгу
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### См. также

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


