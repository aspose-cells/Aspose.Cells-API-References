---
title: "DataModelConnection.ClassType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelConnection özelliği. Bu ExternalConnection nesnesinin türünü alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/datamodelconnection/classtype/
---
## DataModelConnection.ClassType property

Bu [`ExternalConnection`](../../externalconnection/) nesnesinin tipini alır.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.QueryTables;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Başlatılmamış nesneyi kullanarak DataModelConnection örneği oluştur
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

            // Geçerli ClassType değerini göster (yalnızca okuma özelliği)
            Console.WriteLine("Current ClassType value: " + connection.ClassType);

            // Bağlantı özelliklerini ayarla
            connection.Command = "SELECT * FROM Products";
            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            // ClassType'ın bağlantı yönetimini nasıl etkilediğini göster
            if (connection.ClassType == ExternalConnectionClassType.DataModel)
            {
                Console.WriteLine("This is a Data Model connection");
                // Veri modeli bağlantısı için PowerQueryFormula ekle
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
                PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
                query.Name = "ProductQuery";
                typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
                ((IList<PowerQueryFormula>)queries).Add(query);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


