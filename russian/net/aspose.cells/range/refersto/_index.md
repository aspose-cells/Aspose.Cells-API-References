---
title: "Range.RefersTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Range. Получает диапазоны, на которые ссылается"
type: docs
url: /ru/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Получает значение свойства RefersTo диапазона.

```csharp
public string RefersTo { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Создать именованный диапазон
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // Установите свойство RefersTo для именованного диапазона
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Получите диапазоны, на которые ссылается имя
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // Отобразите свойство RefersTo первого диапазона
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // Создайте формулу, использующую именованный диапазон
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // Вычислить формулу
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### См. также

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


