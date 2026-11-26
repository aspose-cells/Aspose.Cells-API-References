---
title: "PowerQueryFormula.Description"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormula. Получает и задает описание формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformula/description/
---
## PowerQueryFormula.Description property

Получает и задает описание формулы Power Query.

```csharp
public string Description { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaPropertyDescriptionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Загрузить существующий файл с формулами Power Query
                workbook = new Workbook("example.xlsx");

                // Получить доступ к существующим формулам Power Query
                if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
                {
                    PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];

                    // Отобразить текущее значение Description
                    Console.WriteLine("Current Description: " + formula.Description);

                    // Установить новое описание
                    formula.Description = "This is an updated description for the Power Query formula";
                    Console.WriteLine("Updated Description: " + formula.Description);

                    // Сохраните книгу
                    workbook.Save("PowerQueryFormulaDescriptionDemo.xlsx");
                    Console.WriteLine("Description property demonstrated successfully.");
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
                Console.WriteLine("Please ensure the example.xlsx file exists and contains Power Query formulas.");
            }
        }
    }
}
```

### См. также

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


