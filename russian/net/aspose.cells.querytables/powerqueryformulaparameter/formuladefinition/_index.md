---
title: "PowerQueryFormulaParameter.FormulaDefinition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaParameter. Возвращает определение параметра"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaparameter/formuladefinition/
---
## PowerQueryFormulaParameter.FormulaDefinition property

Получает определение параметра.

```csharp
public override string FormulaDefinition { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyFormulaDefinitionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получить доступ к свойству DataMashup рабочей книги
                DataMashup dataMashup = workbook.DataMashup;

                if (dataMashup != null)
                {
                    // Получите доступ к коллекции PowerQueryFormulaParameters
                    PowerQueryFormulaParameterCollection parameters = dataMashup.PowerQueryFormulaParameters;

                    // Перебрать параметры, чтобы продемонстрировать FormulaDefinition
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Отобразить значение свойства FormulaDefinition (только для чтения)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Formula Definition: {parameter.FormulaDefinition}");
                        Console.WriteLine($"Parameter Value: {parameter.Value}");
                        Console.WriteLine("----------------------------------------");
                    }

                    if (parameters.Count == 0)
                    {
                        Console.WriteLine("No PowerQueryFormulaParameter instances found in the workbook.");
                    }
                }
                else
                {
                    Console.WriteLine("No DataMashup available in the workbook.");
                }

                // Сохраните книгу
                workbook.Save("FormulaDefinitionDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


