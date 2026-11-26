---
title: "Cell.R1C1Formula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Получает или задает формулу R1C1 ячейки"
type: docs
url: /ru/net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Получает или задает формулу R1C1 объекта [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyR1C1FormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите значение A1
            worksheet.Cells["A1"].PutValue(10);
            
            // Установите значение B1
            worksheet.Cells["B1"].PutValue(20);
            
            // Установите формулу C1 в нотации A1
            worksheet.Cells["C1"].Formula = "=A1+B1";
            
            // Получить и отобразить формулу R1C1
            string r1c1Formula = worksheet.Cells["C1"].R1C1Formula;
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
            
            // Установите формулу D1 в нотации R1C1
            worksheet.Cells["D1"].R1C1Formula = "=RC[-3]+RC[-2]";
            
            // Получить и отобразить формулу A1
            string a1Formula = worksheet.Cells["D1"].Formula;
            Console.WriteLine("A1 Formula: " + a1Formula);
            
            // Сохраните книгу
            workbook.Save("R1C1FormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


