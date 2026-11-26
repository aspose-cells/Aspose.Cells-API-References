---
title: "Range.IsBlank"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Указывает, содержит ли диапазон значения"
type: docs
url: /ru/net/aspose.cells/range/isblank/
---
## Range.IsBlank method

Указывает, содержит ли диапазон значения.

```csharp
public bool IsBlank()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте диапазон и проверьте, пуст ли он (должно быть true)
            Aspose.Cells.Range range1 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank: " + range1.IsBlank());

            // Поместите значение в одну ячейку и проверьте снова (должно быть false)
            cells["B2"].PutValue("Test");
            Aspose.Cells.Range range2 = cells.CreateRange("A1:C10");
            Console.WriteLine("Range A1:C10 is blank after adding value: " + range2.IsBlank());
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


