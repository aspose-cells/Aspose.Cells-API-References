---
title: "PowerQueryFormula.PowerQueryFormulaItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormula. Получает все элементы формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/
---
## PowerQueryFormula.PowerQueryFormulaItems property

Получает все элементы формулы Power Query.

```csharp
public PowerQueryFormulaItemCollection PowerQueryFormulaItems { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyPowerQueryFormulaItemsDemo
    {
        public static void Run()
        {
            // Загрузить исходную книгу
            Workbook workbook = new Workbook("example.xlsx");

            // Получить первую формулу Power Query и её первый элемент
            PowerQueryFormulaItem item = workbook.DataMashup.PowerQueryFormulas[0].PowerQueryFormulaItems[0];
            
            // Изменить значение элемента (заменить букву диска)
            string modifiedValue = item.Value.Replace(@"C:\", @"D:\");
            item.Value = modifiedValue;

            // Сохраните книгу
            workbook.Save("modified_example.xlsx");

            // Проверьте изменение
            Console.WriteLine("Original value modified to: " + modifiedValue);
        }
    }
}
```

### См. также

* class [PowerQueryFormulaItemCollection](../../powerqueryformulaitemcollection/)
* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


