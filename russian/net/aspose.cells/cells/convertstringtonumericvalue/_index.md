---
title: "Cells.ConvertStringToNumericValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Преобразует все строковые данные в листе в числовые значения, если это возможно"
type: docs
url: /ru/net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Преобразует все строковые данные в листе в числовое значение, если это возможно.

```csharp
public void ConvertStringToNumericValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodConvertStringToNumericValueDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Поместите строковые значения, которые могут быть преобразованы в числовые значения
            cells[0, 0].PutValue("1.23");
            cells[0, 1].PutValue("1.24");
            cells[0, 2].PutValue("1.23");
            cells[0, 3].PutValue("6/20/2021");
            cells[0, 4].PutValue("def"); // This will remain as string
            cells[0, 5].PutValue("6/20/2021");

            // Преобразуйте строковые значения в числовые, где это возможно
            cells.ConvertStringToNumericValue();

            // Отобразите преобразованные значения
            Console.WriteLine("A1: " + cells[0, 0].DoubleValue);
            Console.WriteLine("B1: " + cells[0, 1].DoubleValue);
            Console.WriteLine("C1: " + cells[0, 2].DoubleValue);
            Console.WriteLine("D1: " + cells[0, 3].DoubleValue);
            Console.WriteLine("E1: " + cells[0, 4].StringValue); // Remains as string
            Console.WriteLine("F1: " + cells[0, 5].DoubleValue);
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


