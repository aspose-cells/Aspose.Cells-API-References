---
title: "PowerQueryFormula.GroupName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PowerQueryFormula. Получает имя группы, содержащей эту формулу Power Query"
type: docs
url: /ru/net/aspose.cells.querytables/powerqueryformula/groupname/
---
## PowerQueryFormula.GroupName property

Получает имя группы, содержащей эту формулу Power Query.

```csharp
public string GroupName { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class PowerQueryFormulaPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте формулу Power Query (симулировано, так как мы не можем создавать реальные PowerQueryFormulas напрямую)
            // Обычно вы бы загрузили из существующего файла с формулами Power Query
            string sourcePath = "example.xlsx";
            
            try
            {
                workbook = new Workbook(sourcePath);
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                
                if (queries.Count > 0)
                {
                    Console.WriteLine("First Power Query Formula Group Name: " + queries[0].GroupName);
                    
                    // Продемонстрировать доступ к свойству GroupName
                    string groupName = queries[0].GroupName;
                    Console.WriteLine($"Group Name: {groupName}");
                    
                    // Сохраните и перезагрузите, чтобы продемонстрировать сохранность
                    string destPath = "output.xlsx";
                    workbook.Save(destPath);
                    
                    Workbook workbook2 = new Workbook(destPath);
                    PowerQueryFormulaCollection queries2 = workbook2.DataMashup.PowerQueryFormulas;
                    if (queries2.Count > 0)
                    {
                        Console.WriteLine("After reload - Group Name: " + queries2[0].GroupName);
                    }
                }
                else
                {
                    Console.WriteLine("No Power Query formulas found in the file.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
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


