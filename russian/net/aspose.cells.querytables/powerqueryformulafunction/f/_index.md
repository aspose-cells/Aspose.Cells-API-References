---
title: "PowerQueryFormulaFunction.F"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaFunction. Возвращает и задает определение функции"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulafunction/f/
---
## PowerQueryFormulaFunction.F property

Получает и задает определение функции.

```csharp
public string F { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaFunctionPropertyFDemo
    {
        public static void Run()
        {
            // Загрузить книгу, содержащую существующие формулы Power Query
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к коллекции формул Power Query
            PowerQueryFormulaCollection queryFormulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Получить существующую формулу функции по имени
            PowerQueryFormula formula = queryFormulas["from_timestamp"];
            
            // Привести к PowerQueryFormulaFunction для доступа к свойству F
            if (formula is PowerQueryFormulaFunction function)
            {
                // Продемонстрировать получение свойства F
                Console.WriteLine("Original Function Definition: " + function.F);
                
                // Продемонстрировать установку свойства F
                function.F = "(x as number) as datetimezone => #datetimezone(1970,1,1,0,0,0,0,0) + #duration(0,0,0,x)";
                Console.WriteLine("Updated Function Definition: " + function.F);
            }
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


