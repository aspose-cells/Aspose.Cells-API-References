---
title: "DBConnection.ClassType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DBConnection özelliği. Bu ExternalConnection nesnesinin tipini alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

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
    using System;

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // DBConnection örneğini koleksiyona ekleyerek yeni bir DBConnection nesnesi oluştur.
                // DBConnection'ın genel parametresiz bir yapıcıya sahip olmaması nedeniyle,
                // koleksiyonun bizim için oluşturmasına izin vereceğiz
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // ClassType değerini gösterin (yalnızca okuma özelliği)
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // Örneği daha anlamlı kılmak için diğer özelliklerin ayarlanmasını gösterin
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // Çalışma kitabını kaydedin
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


