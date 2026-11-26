---
title: "PowerQueryFormulaFunction.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaFunction. Возвращает тип формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

Получает тип формулы Power Query.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать функцию формулы Power Query
            // Поскольку мы не можем создать напрямую, нам потребуется получить её откуда‑то
            // Для демонстрационных целей мы просто покажем, как получить доступ к свойству Type
            // (В реальном использовании вы бы получили это из существующей коллекции)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // Поскольку мы также не можем создать QueryTable напрямую, мы пропустим эту часть
            QueryTable queryTable = null; // Can't instantiate directly
            
            // Нельзя добавить в коллекцию query tables таким способом — она только для чтения
            // worksheet.QueryTables[0] = queryTable; // Удалена эта строка
            
            // Для демонстрации мы просто покажем формат вывода, который бы использовали, если бы у нас была функция
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // Сохранить результат
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


