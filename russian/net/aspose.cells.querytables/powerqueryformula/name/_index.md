---
title: "PowerQueryFormula.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormula. Получает и задает имя формулы Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Получает и задает имя формулы Power Query.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Загрузить существующий файл с формулами Power Query
            workbook = new Workbook("example.xlsx");
            
            // Получить доступ к существующим формулам Power Query
            if (workbook.DataMashup.PowerQueryFormulas.Count > 0)
            {
                PowerQueryFormula formula = workbook.DataMashup.PowerQueryFormulas[0];
                
                // Продемонстрировать использование свойства Name
                Console.WriteLine("Original Power Query Formula Name: " + formula.Name);
                
                // Изменить имя
                formula.Name = "UpdatedSalesFilter";
                Console.WriteLine("Updated Power Query Formula Name: " + formula.Name);
                
                // Сохраните книгу
                workbook.Save("PowerQueryFormulaDemo.xlsx");
            }
            else
            {
                Console.WriteLine("No Power Query formulas found in the workbook.");
            }
        }
    }
}
```

### См. также

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


