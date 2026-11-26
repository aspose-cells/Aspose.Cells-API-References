---
title: "Перечисление LookAtType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LookAtType enum. Представляет тип поиска"
type: docs
url: /ru/net/aspose.cells/lookattype/
---
## LookAtType enumeration

Представляет тип look at.

```csharp
public enum LookAtType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Contains | `0` | Значение ячейки содержит искомый объект. |
| StartWith | `1` | Значение ячейки начинается с искомого объекта. |
| EndWith | `2` | Значение ячейки заканчивается искомым объектом. |
| EntireContent | `3` | Значение ячейки совпадает с искомым объектом. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LookAtTypeDemo
    {
        public static void LookAtTypeExample()
        {
            // Создайте объект рабочей книги
            Workbook workbook = new Workbook("LookAtTypeExample_original.xlsx");

            // Получить коллекцию Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // Создайте объект FindOptions
            FindOptions findOptions = new FindOptions();

            // Создайте область Cells
            CellArea ca = new CellArea();
            ca.StartRow = 8;
            ca.StartColumn = 2;
            ca.EndRow = 17;
            ca.EndColumn = 13;

            // Установите область ячеек для параметров поиска
            findOptions.SetRange(ca);

            // Установите свойства поиска
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // Установите LookAtType в Contains
            findOptions.LookAtType = LookAtType.Contains;

            // Найдите ячейку с определённым значением
            Cell cell = cells.Find("searchValue", null, findOptions);

            if (cell != null)
            {
                Console.WriteLine($"Cell found at row {cell.Row}, column {cell.Column}");
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


