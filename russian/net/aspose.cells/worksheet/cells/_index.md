---
title: "Worksheet.Cells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает коллекцию Cells"
type: docs
url: /ru/net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Получает коллекцию [`Cells`](../../cells/).

```csharp
public Cells Cells { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Доступ к коллекции cells
            Cells cells = worksheet.Cells;
            
            // Установить значения в cells
            cells["A1"].PutValue("Item");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);
            
            // Установить формулу для вычисления итога
            cells["A4"].PutValue("Total:");
            cells["B4"].Formula = "=SUM(B2:B3)";
            
            // Вычислить формулы
            workbook.CalculateFormula();
            
            // Отобразить значения ячеек
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);
            Console.WriteLine("B2: " + cells["B2"].StringValue);
            Console.WriteLine("A3: " + cells["A3"].StringValue);
            Console.WriteLine("B3: " + cells["B3"].StringValue);
            Console.WriteLine("A4: " + cells["A4"].StringValue);
            Console.WriteLine("B4: " + cells["B4"].StringValue + " (Formula: " + cells["B4"].Formula + ")");
            
            // Сохранить книгу
            workbook.Save("CellsPropertyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


