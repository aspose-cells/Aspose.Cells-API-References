---
title: "DBConnection.SecondCommand"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DBConnection özelliği. PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci bir komut metni dizesi belirtir. ODBC bağlantıları için serverCommand genellikle komuttan daha geniş bir sorgudur; önceki sorguda WHERE koşulu bulunmaz. Bu iki komut (Command ve ServerCommand) temelinde parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir"
type: docs
url: /tr/net/aspose.cells.externalconnections/dbconnection/secondcommand/
---
## DBConnection.SecondCommand property

PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metin dizesini belirtir. ODBC bağlantıları için serverCommand genellikle command'tan daha geniş bir sorgudur (ilkinde WHERE koşulu bulunmaz). Bu iki komuta (Command ve ServerCommand) dayanarak, parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir.

```csharp
public override string SecondCommand { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // DBConnection örneğini koleksiyona ekleyerek yeni bir DBConnection nesnesi oluştur.
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[0];
                
                // Temel bir bağlantı kurun
                dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
                dbConnection.CommandType = OLEDBCommandType.SqlStatement;
                dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
                
                // SecondCommand özelliğini ayarlayın ve gösterin
                dbConnection.SecondCommand = "SELECT * FROM Customers";
                Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
                
                // SecondCommand özelliğini değiştirerek yazılabilir olduğunu gösterin
                dbConnection.SecondCommand = "SELECT * FROM Orders";
                Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
                
                // Çalışma kitabını kaydedin
                workbook.Save("SecondCommandDemo.xlsx");
                
                Console.WriteLine("SecondCommand demonstration completed successfully.");
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


