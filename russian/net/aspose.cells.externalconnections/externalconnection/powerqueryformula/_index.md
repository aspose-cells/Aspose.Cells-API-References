---
title: "ExternalConnection.PowerQueryFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Получает определение формулы Power Query"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Получает определение формулы Power Query.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.QueryTables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Загрузить существующую книгу с соединениями данных для демонстрации PowerQueryFormula
            workbook = new Workbook("example.xlsx");
            
            // Получить доступ к существующему соединению (предполагая, что у книги есть хотя бы одно соединение)
            if (workbook.DataConnections.Count > 0)
            {
                var connection = workbook.DataConnections[0];
                Console.WriteLine("Power Query Formula Demo:");
                Console.WriteLine($"Connection Name: {connection.Name}");
                
                // Получить доступ к свойству PowerQueryFormula
                PowerQueryFormula powerQuery = connection.PowerQueryFormula;
                if (powerQuery != null)
                {
                    Console.WriteLine($"Formula Name: {powerQuery.Name}");
                    Console.WriteLine($"Formula Definition: {powerQuery.FormulaDefinition}");
                }
                else
                {
                    Console.WriteLine("No Power Query Formula found for this connection");
                }
            }
            else
            {
                Console.WriteLine("No data connections found in the workbook");
            }
            
            // Сохраните книгу
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


