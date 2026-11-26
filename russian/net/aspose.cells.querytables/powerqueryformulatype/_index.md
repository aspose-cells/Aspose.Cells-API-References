---
title: "Перечисление PowerQueryFormulaType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.QueryTables.PowerQueryFormulaType. Представляет тип формулы Power Query."
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulatype/
---
## PowerQueryFormulaType enumeration

Представляет тип формулы Power Query.

```csharp
public enum PowerQueryFormulaType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Formula | `0` | Формула Power Query. |
| Function | `1` | Функция Power Query. |
| Parameter | `2` | Параметр Power Query. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Продемонстрировать все значения перечисления PowerQueryFormulaType
                PowerQueryFormulaType formulaType = PowerQueryFormulaType.Formula;
                PowerQueryFormulaType functionType = PowerQueryFormulaType.Function;
                PowerQueryFormulaType parameterType = PowerQueryFormulaType.Parameter;

                // Отобразить значения перечисления и их числовые представления
                Console.WriteLine($"Formula type: {formulaType} ({(int)formulaType})");
                Console.WriteLine($"Function type: {functionType} ({(int)functionType})");
                Console.WriteLine($"Parameter type: {parameterType} ({(int)parameterType})");

                // Продемонстрировать сравнение перечислений
                if (formulaType == PowerQueryFormulaType.Formula)
                {
                    Console.WriteLine("Successfully identified Formula type");
                }

                if (functionType == PowerQueryFormulaType.Function)
                {
                    Console.WriteLine("Successfully identified Function type");
                }

                if (parameterType == PowerQueryFormulaType.Parameter)
                {
                    Console.WriteLine("Successfully identified Parameter type");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormulaType: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


