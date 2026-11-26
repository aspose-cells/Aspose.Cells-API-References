---
title: "Класс PowerQueryFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.QueryTables.PowerQueryFormula класс. Представляет определение формулы Power Query."
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Представляет определение формулы Power Query.

```csharp
public class PowerQueryFormula
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Получает и задает описание формулы Power Query. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Получает определение формулы Power Query. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Получает имя группы, содержащей эту формулу Power Query. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Получает и задает имя формулы Power Query. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Получает все элементы формулы Power Query. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Получает тип этой формулы Power Query. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class QueryTablesClassPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Получите доступ к коллекции PowerQueryFormulas из DataMashup
                PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;

                // Проверьте, существуют ли какие‑либо формулы
                if (formulas.Count > 0)
                {
                    // Получите первую PowerQueryFormula
                    PowerQueryFormula formula = formulas[0];

                    // Отобразить свойства только для чтения
                    Console.WriteLine($"Formula Type: {formula.Type}");
                    Console.WriteLine($"Group Name: {formula.GroupName}");
                    Console.WriteLine($"Formula Definition: {formula.FormulaDefinition}");

                    // Отобразите и измените свойства с чтением и записью
                    Console.WriteLine($"Original Name: {formula.Name}");
                    formula.Name = "ModifiedFormulaName";
                    Console.WriteLine($"Modified Name: {formula.Name}");

                    Console.WriteLine($"Original Description: {formula.Description}");
                    formula.Description = "Updated description for the formula";
                    Console.WriteLine($"Modified Description: {formula.Description}");

                    // Отобразите количество элементов формулы
                    Console.WriteLine($"Number of Formula Items: {formula.PowerQueryFormulaItems.Count}");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    Console.WriteLine("This is expected for a new workbook.");
                }

                // Сохраните книгу
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PowerQueryFormula: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


