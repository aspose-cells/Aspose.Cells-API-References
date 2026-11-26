---
title: "PowerQueryFormulaItemCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaItemCollection. Возвращает PowerQueryFormulaItem по индексу в списке"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaitemcollection/item/
---
## PowerQueryFormulaItemCollection indexer (1 of 2)

Возвращает [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) по индексу в списке.

```csharp
public PowerQueryFormulaItem this[int index] { get; }
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
    public class PowerQueryFormulaItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу с шаблоном, содержащим Power Query
            Workbook workbook = new Workbook();
            
            // Получить первую формулу Power Query (если она существует)
            var powerQueryFormula = workbook.DataMashup.PowerQueryFormulas[0];
            
            // Изменить элементы формулы, используя свойство Item
            var formulaItems = powerQueryFormula.PowerQueryFormulaItems;
            if (formulaItems.Count > 0)
            {
                formulaItems[0].Value = "Sql.Database(\"SQL2K16\", \"EUC876REG\", [Query=\"select * from CANOTIFICATIONS\"])";
                
                // Проверьте изменение
                Console.WriteLine(formulaItems[0].Value);
            }
            
            // Сохраните книгу
            workbook.Save("PowerQueryExample.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)

---

## PowerQueryFormulaItemCollection indexer (2 of 2)

Возвращает [`PowerQueryFormulaItem`](../../powerqueryformulaitem/) по имени элемента.

```csharp
public PowerQueryFormulaItem this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя элемента. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            try
            {
                // Загрузить книгу, содержащую формулы Power Query.
                // Замените путь на реальный файл, содержащий Power Query, если он доступен.
                string sourcePath = "PowerQuerySample.xlsx";
                Workbook workbook = System.IO.File.Exists(sourcePath) ? new Workbook(sourcePath) : new Workbook();

                // Получить доступ к коллекции формул Power Query.
                PowerQueryFormulaCollection pqFormulas = workbook.DataMashup.PowerQueryFormulas;

                if (pqFormulas.Count == 0)
                {
                    Console.WriteLine("No Power Query formulas found in the workbook.");
                    return;
                }

                // Получить первую формулу Power Query.
                PowerQueryFormula formula = pqFormulas[0];

                // Получить доступ к её коллекции элементов.
                PowerQueryFormulaItemCollection items = formula.PowerQueryFormulaItems;

                if (items.Count == 0)
                {
                    Console.WriteLine("The selected Power Query formula contains no items.");
                    return;
                }

                // Получить первый элемент, чтобы получить корректное имя элемента.
                PowerQueryFormulaItem firstItem = items[0];
                string itemName = firstItem.Name;

                // Использовать индексатор Item(string) (только для чтения), чтобы получить тот же элемент по имени.
                PowerQueryFormulaItem retrievedItem = items[itemName];

                // Отобразить свойства полученного элемента.
                Console.WriteLine($"Item Name : {retrievedItem.Name}");
                Console.WriteLine($"Item Value: {retrievedItem.Value}");
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

* class [PowerQueryFormulaItem](../../powerqueryformulaitem/)
* class [PowerQueryFormulaItemCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


