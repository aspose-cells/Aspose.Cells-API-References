---
title: "Range.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Получает и задает значение диапазона."
type: docs
url: /ru/net/aspose.cells/range/value/
---
## Range.Value property

Получает и задает значение диапазона.

```csharp
public object Value { get; set; }
```

### Примечания

Если диапазон содержит несколько ячеек, возвращаемый/применяемый объект должен быть двумерным массивом.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать диапазон, начинающийся с A1 и охватывающий 3×3 ячейки.
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");

            // Установить двумерный массив в качестве значения диапазона.
            int[,] values = new int[3, 3] { { 1, 2, 3 }, { 4, 5, 6 }, { 7, 8, 9 } };
            range.Value = values;

            // Сохраните книгу
            workbook.Save("RangePropertyValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


