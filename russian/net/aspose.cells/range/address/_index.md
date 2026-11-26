---
title: "Range.Address"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Получает адрес диапазона"
type: docs
url: /ru/net/aspose.cells/range/address/
---
## Range.Address property

Получает адрес диапазона.

```csharp
public string Address { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyAddressDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте диапазон и продемонстрируйте свойство Address
            Aspose.Cells.Range range = cells.CreateRange("A1");
            Console.WriteLine("Original range address: " + range.Address);

            // Продемонстрировать GetOffset с Address
            Aspose.Cells.Range offsetRange = range.GetOffset(1, 1);
            Console.WriteLine("Offset range address: " + offsetRange.Address);

            // Продемонстрировать адрес EntireRow
            Aspose.Cells.Range entireRow = range.EntireRow;
            Console.WriteLine("Entire row address: " + entireRow.Address);

            // Продемонстрировать адрес EntireColumn
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            Console.WriteLine("Entire column address: " + entireColumn.Address);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


