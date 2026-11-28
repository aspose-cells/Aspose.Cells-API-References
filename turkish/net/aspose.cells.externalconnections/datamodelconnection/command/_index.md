---
title: "DataModelConnection.Command"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataModelConnection özelliği. Veri sağlayıcı API'sine geçecek ve harici kaynakla etkileşime girerek veri almak için kullanılan veritabanı komutunu içeren dize."
type: docs
url: /tr/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

Veri sağlayıcı API'sine dış kaynağa etkileşimde bulunarak veri almak için gönderilecek veritabanı komutunu içeren dize.

```csharp
public override string Command { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
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

                // İlk Command değerini göster (boş)
                Console.WriteLine("Initial Command: " + connection.Command);

                // Command özelliğini ayarla
                connection.Command = "SELECT * FROM Customers";
                
                // Güncellenmiş Command değerini göster
                Console.WriteLine("Updated Command: " + connection.Command);

                // Tam bir bağlantı için diğer gerekli özellikleri ayarla
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Bağlantıyla birlikte çalışma kitabını kaydet
                workbook.Save("CommandDemo.xlsx");
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


