---
title: "DBConnection.ConnectionString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DBConnection özelliği. Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır"
type: docs
url: /tr/net/aspose.cells.externalconnections/dbconnection/connectionstring/
---
## DBConnection.ConnectionString property

Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır.

```csharp
public override string ConnectionString { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Harici bağlantıların koleksiyonuna erişin
                ExternalConnectionCollection connections = workbook.DataConnections;

                // DBConnection'ı koleksiyona ekleyerek yeni bir DBConnection oluşturun
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // İlk ConnectionString değerini gösterin
                Console.WriteLine("Initial ConnectionString: " + dbConnection.ConnectionString);

                // Yeni bir bağlantı dizesi ayarlayın
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";

                // Güncellenmiş ConnectionString değerini gösterin
                Console.WriteLine("Updated ConnectionString: " + dbConnection.ConnectionString);

                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionStringDemo.xlsx");
                Console.WriteLine("ConnectionString demonstration completed successfully.");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


