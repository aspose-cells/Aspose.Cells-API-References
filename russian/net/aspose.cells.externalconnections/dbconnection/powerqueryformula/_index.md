---
title: "DBConnection.PowerQueryFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DBConnection. Получает определение формулы Power Query"
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/powerqueryformula/
---
## DBConnection.PowerQueryFormula property

Получает определение формулы Power Query.

```csharp
public override PowerQueryFormula PowerQueryFormula { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;

    public class DBConnectionPropertyPowerQueryFormulaDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            try
            {
                // Получите доступ к коллекции внешних соединений
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Найдите первое DBConnection в коллекции (если есть)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Получите доступ к свойству PowerQueryFormula (только для чтения)
                    PowerQueryFormula powerQueryFormula = dbConn.PowerQueryFormula;

                    if (powerQueryFormula != null)
                    {
                        // Отобразите свойства PowerQueryFormula
                        Console.WriteLine("PowerQueryFormula Type: " + powerQueryFormula.Type);
                        Console.WriteLine("PowerQueryFormula GroupName: " + powerQueryFormula.GroupName);
                        Console.WriteLine("PowerQueryFormula FormulaDefinition: " + powerQueryFormula.FormulaDefinition);
                        Console.WriteLine("PowerQueryFormula Name: " + powerQueryFormula.Name);
                        Console.WriteLine("PowerQueryFormula Description: " + powerQueryFormula.Description);

                        // Продемонстрируйте доступ к коллекции PowerQueryFormulaItems
                        Console.WriteLine("Number of PowerQueryFormulaItems: " + powerQueryFormula.PowerQueryFormulaItems.Count);
                    }
                    else
                    {
                        Console.WriteLine("PowerQueryFormula is null for this connection.");
                    }
                }

                // Сохраните книгу
                workbook.Save("PowerQueryFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved as PowerQueryFormulaDemo.xlsx");
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

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


