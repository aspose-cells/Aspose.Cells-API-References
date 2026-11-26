---
title: "PowerQueryFormulaParameter.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaParameter. Возвращает значение параметра"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaparameter/value/
---
## PowerQueryFormulaParameter.Value property

Получает значение параметра.

```csharp
public string Value { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyValueDemo
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

                    // Итерируйте параметры, чтобы продемонстрировать свойство Value
                    foreach (PowerQueryFormulaParameter parameter in parameters)
                    {
                        // Отобразите текущее значение свойства Value (операция чтения)
                        Console.WriteLine($"Parameter Name: {parameter.Name}");
                        Console.WriteLine($"Current Value: {parameter.Value}");

                        // Поскольку свойство Value доступно для чтения и записи, продемонстрируйте установку нового значения
                        string newValue = "UpdatedValue_" + Guid.NewGuid().ToString();
                        parameter.Value = newValue;
                        Console.WriteLine($"Updated Value: {parameter.Value}");
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
                workbook.Save("ValueDemo.xlsx");
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


