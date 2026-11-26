---
title: "Range.Transpose"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Range. Транспонирование вращает данные из строк в столбцы или наоборот"
type: docs
url: /ru/net/aspose.cells/range/transpose/
---
## Range.Transpose method

Транспонировать (повернуть) данные из строк в столбцы или наоборот.

```csharp
public void Transpose()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodTransposeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните примерными данными диапазон 3x3 (A1:C3)
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].PutValue(6);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["C3"].PutValue(9);
            
            // Создайте диапазон (A1:C3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            
            // Транспонируйте диапазон
            range.Transpose();
            
            // Сохраните книгу
            workbook.Save("TransposedOutput.xlsx");
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


