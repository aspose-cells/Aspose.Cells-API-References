---
title: "ErrorCheckOption.RemoveRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ErrorCheckOption. Удаляет один диапазон по указанному индексу"
type: docs
url: /ru/net/aspose.cells/errorcheckoption/removerange/
---
## ErrorCheckOption.RemoveRange method

Удаляет один диапазон по заданному индексу.

```csharp
public void RemoveRange(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс диапазона, который нужно удалить. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ErrorCheckOptionMethodRemoveRangeWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ErrorCheckOptionCollection errorCheckOptions = worksheet.ErrorCheckOptions;

            // Создайте новый ErrorCheckOption и включите проверку EmptyCellRef
            int optionIndex = errorCheckOptions.Add();
            ErrorCheckOption errorCheckOption = errorCheckOptions[optionIndex];
            errorCheckOption.SetErrorCheck(ErrorCheckType.EmptyCellRef, true);

            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            int rangeIndex = errorCheckOption.AddRange(area);
            int initialCount = errorCheckOption.GetCountOfRange();

            try
            {
                errorCheckOption.RemoveRange(rangeIndex);
                int finalCount = errorCheckOption.GetCountOfRange();
                Console.WriteLine($"Ranges before removal: {initialCount}, after removal: {finalCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveRange: {ex.Message}");
            }

            workbook.Save("ErrorCheckOptionRemoveRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


