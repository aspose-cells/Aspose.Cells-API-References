---
title: "PowerQueryFormulaItem.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormulaItem. Получает имя элемента"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformulaitem/name/
---
## PowerQueryFormulaItem.Name property

Получает имя элемента.

```csharp
public string Name { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaItemPropertyNameDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить пример данных Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            
            // Сохранить, чтобы инициировать создание Power Query
            string sourcePath = "pq_source.xlsx";
            workbook.Save(sourcePath);
            
            // Открыть заново, чтобы получить доступ к формулам Power Query
            workbook = new Workbook(sourcePath);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            
            // Обработать формулы Power Query
            foreach (Aspose.Cells.QueryTables.PowerQueryFormula formula in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine("Formula Name: " + formula.Name);
                
                foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
                {
                    Console.WriteLine("  Item Name: " + item.Name);
                    
                    // Продемонстрировать использование свойства Name
                    if (item.Name == "Source")
                    {
                        Console.WriteLine("Original Value: " + item.Value);
                        item.Value = "ModifiedSource";
                        Console.WriteLine("Modified Value: " + item.Value);
                    }
                }
            }
            
            // Сохранить изменённую книгу
            workbook.Save("pq_modified.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


