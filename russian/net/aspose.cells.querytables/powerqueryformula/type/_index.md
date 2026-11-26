---
title: "PowerQueryFormula.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormula. Получает тип этой формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformula/type/
---
## PowerQueryFormula.Type property

Получает тип этой формулы Power Query.

```csharp
public virtual PowerQueryFormulaType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить существующие формулы (в новой книге их нет) для демонстрации свойства Type
            var formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // В реальном сценарии с существующими формулами мы бы проверяли их типы
            Console.WriteLine("Power Query Formula Types:");
            
            // Это демонстрирует проверку свойства Type
            foreach (PowerQueryFormula formula in formulas)
            {
                Console.WriteLine($"- {formula.Name}: {formula.Type}");
            }

            // Для демонстрационных целей добавить вывод, когда формулы отсутствуют
            if (formulas.Count == 0)
            {
                Console.WriteLine("No power query formulas found in the workbook.");
                Console.WriteLine("Example formula types would be:");
                Console.WriteLine("- Function: " + PowerQueryFormulaType.Function);
                Console.WriteLine("- Parameter: " + PowerQueryFormulaType.Parameter);
                Console.WriteLine("- Formula: " + PowerQueryFormulaType.Formula);
            }

            // Сохраните книгу
            workbook.Save("PowerQueryFormulaTypes.xlsx");
        }
    }
}
```

### См. также

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


