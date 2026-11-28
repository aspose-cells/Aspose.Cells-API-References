---
title: "DataModelConnection.CommandType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelConnection özelliği. OLEDBCommandType türünü döndürür"
type: docs
url: /tr/net/aspose.cells.externalconnections/datamodelconnection/commandtype/
---
## DataModelConnection.CommandType property

[`OLEDBCommandType`](../../oledbcommandtype/) türünü döndürür.

```csharp
public override OLEDBCommandType CommandType { get; set; }
```

### Örnekler

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
            
            // Başlatılmamış nesneyi kullanarak DataModelConnection örneği oluştur
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
            
            Console.WriteLine("Current CommandType value: " + connection.CommandType);

            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.Command = "SELECT * FROM Customers";
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
            string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
            // Başlatılmamış nesneyi kullanarak PowerQueryFormula oluştur ve özellikleri ayarla
            PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
            query.Name = "SampleQuery";
            typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
            ((IList<PowerQueryFormula>)queries).Add(query);

            workbook.Save("PropertyCommandTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


