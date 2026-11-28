---
title: "ExternalConnection.SavePassword"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Parola, bağlantı dizesinin bir parçası olarak kaydedilecekse True, aksi takdirde False"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

Parola bağlantı dizesinin bir parçası olarak kaydedilecekse doğru; aksi takdirde Yanlış.

```csharp
public bool SavePassword { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySavePasswordDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];

                // Mevcut SavePassword değerini göster
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // Özelliği ayarlamayı gösterin (okuma-yazma olduğu için)
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // Değeri değiştirerek ayar yeteneğini göster
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("SavePasswordDemo.xlsx");
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


