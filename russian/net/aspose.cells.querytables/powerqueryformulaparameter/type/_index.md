---
title: "PowerQueryFormulaParameter.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaParameter. Возвращает тип формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

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

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Поскольку мы не можем создать PowerQueryFormulaParameter напрямую, не зная обязательных параметров конструктора,
                // мы продемонстрируем доступ к свойству Type через параметры существующей таблицы запросов
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // В реальном сценарии вы бы получили доступ к этому из существующей таблицы запросов
                // Для демонстрационных целей мы покажем, как проверить тип, если у вас есть экземпляр
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // Отобразите значение свойства Type (только для чтения)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // Показать возможные значения перечисления
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // Сохраните книгу
                workbook.Save("TypeDemo.xlsx");
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

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


