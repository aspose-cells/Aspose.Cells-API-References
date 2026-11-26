---
title: "FormatConditionCollection.RemoveCondition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод FormatConditionCollection. Удаляет условие форматирования по индексу"
type: docs
url: /ru/net/aspose.cells/formatconditioncollection/removecondition/
---
## FormatConditionCollection.RemoveCondition method

Удаляет условие форматирования по индексу.

```csharp
public void RemoveCondition(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс условия форматирования, которое следует удалить. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить коллекцию условий форматирования
            FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
            
            // Добавить несколько примерных условий
            int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
            
            try
            {
                // Отобразить начальное количество
                Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
                
                // Удалить первое условие
                formatConditions.RemoveCondition(index1);
                
                // Отобразить обновленное количество
                Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
                
                // Сохраните книгу
                workbook.Save("RemoveConditionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


