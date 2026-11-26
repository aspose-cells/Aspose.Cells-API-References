---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PowerQueryFormulaCollection. Удалить формулу Power Query по имени"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

Удалить формулу Power Query по имени.

```csharp
public void RemoveBy(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя формулы Power Query. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получите доступ к PowerQueryFormulaCollection (предполагая, что он существует в рабочей книге)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // Добавьте пример формулы для удаления (обычно она берётся из существующих данных)
                string formulaName = "SampleFormula";
                
                // Вызовите RemoveBy с именем формулы
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // Сохраните книгу
                workbook.Save("RemoveByWithStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


