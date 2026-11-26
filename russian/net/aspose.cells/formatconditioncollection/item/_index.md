---
title: "FormatConditionCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FormatConditionCollection. Получает условие форматирования по индексу"
type: docs
url: /ru/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

Получает условие форматирования по индексу.

```csharp
public FormatCondition this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | индекс условия форматирования, которое следует вернуть. |

### Возвращаемое значение

условие форматирования

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавить коллекцию условий форматирования
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // Добавить условие форматирования
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // Получить первое условие форматирования с помощью свойства Item
            FormatCondition condition = fcc[0];
            
            // Отобразить формулы
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // Изменить формулы с помощью свойства Item
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // Отобразить изменённые формулы
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### См. также

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


