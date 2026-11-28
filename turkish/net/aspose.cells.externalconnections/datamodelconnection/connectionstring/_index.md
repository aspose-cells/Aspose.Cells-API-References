---
title: "DataModelConnection.ConnectionString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelConnection özelliği. Bağlantı bilgi dizesi, bir OLE DB veya ODBC veri kaynağıyla iletişim kurmak için kullanılır"
type: docs
url: /tr/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

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
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Başlatılmamış nesneyi kullanarak DataModelConnection örneği oluştur
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // İlk ConnectionString değerini göster (boş)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // ConnectionString özelliğini ayarla
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // Güncellenmiş ConnectionString değerini gösterin
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // Tam bir bağlantı için diğer gerekli özellikleri ayarla
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // Bağlantıyla birlikte çalışma kitabını kaydet
                workbook.Save("ConnectionStringDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


