---
title: "ErrorCheckOption.GetRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ErrorCheckOption. Возвращает диапазон, влияющий на эту настройку, по заданному индексу"
type: docs
url: /ru/net/aspose.cells/errorcheckoption/getrange/
---
## ErrorCheckOption.GetRange method

Получает затронутый диапазон этого параметра по заданному индексу.

```csharp
public CellArea GetRange(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс диапазона |

### Возвращаемое значение

Возвращает влияющий диапазон по заданному индексу.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionMethodGetRangeWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать ErrorCheckOption, используя коллекцию ErrorCheckOptions листа
            int errorCheckIndex = worksheet.ErrorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = worksheet.ErrorCheckOptions[errorCheckIndex];

            CellArea area = new CellArea();
            area.StartRow = 1;
            area.StartColumn = 1;
            area.EndRow = 3;
            area.EndColumn = 3;
            int addedIndex = errorCheckOption.AddRange(area);

            try
            {
                int rangeCount = errorCheckOption.GetCountOfRange();
                if (rangeCount > 0)
                {
                    CellArea retrievedArea = errorCheckOption.GetRange(0);
                    Console.WriteLine($"Retrieved range: StartRow={retrievedArea.StartRow}, StartColumn={retrievedArea.StartColumn}, " +
                        $"EndRow={retrievedArea.EndRow}, EndColumn={retrievedArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRange method: {ex.Message}");
            }

            workbook.Save("ErrorCheckOptionMethodGetRangeWithInt32Demo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


