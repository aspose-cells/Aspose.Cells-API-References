---
title: "CellArea.CompareTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellArea. Сравнивает два объекта CellArea по их верхнему левому углу"
type: docs
url: /ru/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

Сравнивает два объекта CellArea по их левому верхнему углу.

```csharp
public int CompareTo(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object |  |

### Возвращаемое значение

Если два угла находятся в разных строках, сравните их индексы строк. В противном случае сравните их индексы столбцов. Если два угла одинаковы, будет возвращено 0.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // Создать два объекта CellArea для сравнения
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // Продемонстрировать метод CompareTo с параметром Object
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // Создать еще одно сравнение с равными областями
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### См. также

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


