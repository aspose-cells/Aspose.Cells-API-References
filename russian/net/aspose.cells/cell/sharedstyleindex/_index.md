---
title: "Cell.SharedStyleIndex"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает индекс общего стиля ячейки в пуле стилей"
type: docs
url: /ru/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Получает индекс общего стиля ячейки в пуле стилей.

```csharp
public int SharedStyleIndex { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль и задайте некоторые свойства
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // Применить стиль к ячейке A1
            worksheet.Cells["A1"].SetStyle(style);

            // Получите индекс общего стиля ячейки A1
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // Получите стиль из пула стилей, используя индекс
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // Выведите информацию о стиле для проверки
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


