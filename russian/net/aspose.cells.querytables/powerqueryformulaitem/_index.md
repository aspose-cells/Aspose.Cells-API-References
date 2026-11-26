---
title: "Класс PowerQueryFormulaItem"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.QueryTables.PowerQueryFormulaItem класс. Представляет элемент формулы Power Query."
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaitem/
---
## PowerQueryFormulaItem class

Представляет элемент формулы Power Query.

```csharp
public class PowerQueryFormulaItem
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ItemType](../../aspose.cells.querytables/powerqueryformulaitem/itemtype/) { get; } | Получает тип этого элемента (Function, Parameter, List, Literal или Unknown). |
| [Name](../../aspose.cells.querytables/powerqueryformulaitem/name/) { get; } | Получает имя элемента. |
| [TextValue](../../aspose.cells.querytables/powerqueryformulaitem/textvalue/) { get; } | Получает текстовое значение элемента. |
| [Value](../../aspose.cells.querytables/powerqueryformulaitem/value/) { get; set; } | Получает значение элемента. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;

    public class QueryTablesClassPowerQueryFormulaItemDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте новую книгу (может быть существующий файл, если у вас есть данные Power Query)
                Workbook workbook = new Workbook();

                // Получите доступ к объекту DataMashup, содержащему формулы PowerQuery
                DataMashup mashup = workbook.DataMashup;

                bool itemFound = false;

                // Итерируйте все формулы PowerQuery и их элементы
                foreach (PowerQueryFormula formula in mashup.PowerQueryFormulas)
                {
                    foreach (PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                    {
                        // Продемонстрируйте свойство Name только для чтения
                        Console.WriteLine($"Item Name: {item.Name}");

                        // Продемонстрируйте свойство Value с чтением/записью
                        Console.WriteLine($"Original Value: {item.Value}");
                        item.Value = "SampleValue";
                        Console.WriteLine($"Modified Value: {item.Value}");

                        itemFound = true;
                    }
                }

                if (!itemFound)
                {
                    Console.WriteLine("No PowerQueryFormulaItem instances were found in the workbook.");
                }

                Console.WriteLine("PowerQueryFormulaItem demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaItem: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


