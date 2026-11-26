---
title: "PowerQueryFormulaCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaCollection. Получает PowerQueryFormula по индексу в списке"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulacollection/item/
---
## PowerQueryFormulaCollection indexer (1 of 2)

Получает [`PowerQueryFormula`](../../powerqueryformula/) по индексу в списке.

```csharp
public PowerQueryFormula this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить формулы Power Query
            var dataMashup = workbook.DataMashup;
            var formulas = dataMashup.PowerQueryFormulas;
            
            // Создать и добавить новую формулу (при необходимости)
            // Примечание: Реальная реализация может потребовать другого подхода для добавления формул
            // Для демонстрационных целей будем работать с существующими формулами, если они есть
            if (formulas.Count == 0)
            {
                // Это только для демонстрации — реальный API может потребовать другого подхода
                // для создания новых формул
                return;
            }

            // Получите первую формулу, используя свойство Item
            var formula = formulas[0];
            
            // Получить элементы формул
            var formulaItems = formula.PowerQueryFormulaItems;
            if (formulaItems.Count == 0)
            {
                // Это только для демонстрации — реальный API может потребовать другого подхода
                // для создания новых элементов формул
                return;
            }

            // Получите первый элемент, используя свойство Item
            var formulaItem = formulaItems[0];
            
            // Установить и получить значение, используя свойство Item
            string formulaText = "Sql.Database(\"SERVER\", \"DB\", [Query=\"SELECT * FROM TABLE\"])";
            formulaItem.Value = formulaText;
            
            // Продемонстрировать использование свойства Item
            string retrievedValue = formulaItems[0].Value;
            Console.WriteLine("Power Query Formula Item Value: " + retrievedValue);
            
            // Сохраните книгу
            workbook.Save("PowerQueryDemo.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaCollection indexer (2 of 2)

Получает [`PowerQueryFormula`](../../powerqueryformula/) по имени формулы Power Query.

```csharp
public PowerQueryFormula this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя элемента. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создайте рабочую книгу, загрузив существующий файл, содержащий формулы Power Query
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить коллекцию формул Power Query
            PowerQueryFormulaCollection formulas = workbook.DataMashup.PowerQueryFormulas;
            
            // Продемонстрировать использование свойства Item
            try
            {
                // Попробуйте получить доступ к существующей формуле (если есть)
                if (formulas.Count > 0)
                {
                    PowerQueryFormula formula = formulas[formulas[0].Name];
                    Console.WriteLine("First formula found: " + formula.Name);
                    Console.WriteLine("Formula definition: " + formula.FormulaDefinition);
                    Console.WriteLine("Formula type: " + formula.Type);
                }
                
                // Это вызовет исключение для несуществующей формулы
                PowerQueryFormula nonExistent = formulas["NonExistentFormula"];
            }
            catch (Exception ex)
            {
                Console.WriteLine("Expected error accessing non-existent formula: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [PowerQueryFormula](../../powerqueryformula/)
* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


