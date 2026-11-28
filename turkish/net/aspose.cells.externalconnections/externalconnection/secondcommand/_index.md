---
title: "ExternalConnection.SecondCommand"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metin dizesini belirtir. ODBC bağlantıları için serverCommand, komuttan genellikle daha geniş bir sorgudur; önceki sorguda WHERE koşulu bulunmaz. Bu iki komut olan commandsCommand ve ServerCommand parametresi temelinde UI doldurulabilir ve parametreli sorgular oluşturulabilir."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

PivotTable sunucu tabanlı sayfa alanları kullanıldığında kalıcı olan ikinci komut metin dizesini belirtir. ODBC bağlantıları için serverCommand genellikle command'tan daha geniş bir sorgudur (ilkinde WHERE koşulu bulunmaz). Bu iki komuta (Command ve ServerCommand) dayanarak, parametre UI'si doldurulabilir ve parametreli sorgular oluşturulabilir.

```csharp
public virtual string SecondCommand { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mevcut SecondCommand değerini göster (okuma işlemi)
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // Yeni bir SecondCommand değeri ayarla (okuma-yazma olduğu için)
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // Boş dize ayarlamayı göstermek için SecondCommand'i temizle
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("SecondCommandDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


