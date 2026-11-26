---
title: "PowerQueryFormula.FormulaDefinition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormula. Получает определение формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformula/formuladefinition/
---
## PowerQueryFormula.FormulaDefinition property

Получает определение формулы Power Query.

```csharp
public virtual string FormulaDefinition { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyFormulaDefinitionDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать пример таблицы, на которую может ссылаться Power Query
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Test");
            
            // Получить существующие формулы Power Query (будут пустыми в новой книге)
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Получить первую формулу, если она существует (демонстрируя использование FormulaDefinition)
            if (formulas.Count > 0)
            {
                PowerQueryFormula formula = formulas[0];
                Console.WriteLine("Formula Definition: " + formula.FormulaDefinition);
                Console.WriteLine("Formula Name: " + formula.Name);
                Console.WriteLine("Formula Description: " + formula.Description);
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
            
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


