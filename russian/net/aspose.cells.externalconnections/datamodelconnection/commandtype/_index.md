---
title: "DataModelConnection.CommandType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DataModelConnection. Возвращает тип OLEDBCommandType"
type: docs
url: /ru/net/aspose.cells.externalconnections/datamodelconnection/commandtype/
---
## DataModelConnection.CommandType property

Возвращает тип [`OLEDBCommandType`](../../oledbcommandtype/).

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;
    using System.Collections.Generic;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Создать экземпляр DataModelConnection, используя неинициализированный объект
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
            
            Console.WriteLine("Current CommandType value: " + connection.CommandType);

            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.Command = "SELECT * FROM Customers";
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
            string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
            // Создать PowerQueryFormula, используя неинициализированный объект, и установить свойства
            PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
            query.Name = "SampleQuery";
            typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
            ((IList<PowerQueryFormula>)queries).Add(query);

            workbook.Save("PropertyCommandTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


