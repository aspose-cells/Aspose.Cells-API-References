---
title: "Cell.GetFormatConditions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает условия форматирования, которые применяются к этой ячейке."
type: docs
url: /ru/net/aspose.cells/cell/getformatconditions/
---
## Cell.GetFormatConditions method

Получает условия форматирования, применяемые к этой ячейке.

```csharp
public FormatConditionCollection[] GetFormatConditions()
```

### Возвращаемое значение

Возвращает объект [`FormatConditionCollection`](../../formatconditioncollection/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetFormatConditionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить коллекцию ячеек
            Cells cells = worksheet.Cells;
            
            // Добавьте примерные данные
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            
            // Добавьте условие форматирования в ячейку A1
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "15");
            
            // Получите условия форматирования для ячейки A1
            FormatConditionCollection[] conditions = cells["A1"].GetFormatConditions();
            
            // Выведите количество условий форматирования
            Console.WriteLine("Number of format conditions: " + conditions.Length);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FormatConditionCollection](../../formatconditioncollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


