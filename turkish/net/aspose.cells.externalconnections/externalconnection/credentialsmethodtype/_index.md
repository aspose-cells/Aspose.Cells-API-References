---
title: "ExternalConnection.CredentialsMethodType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bağlantıyı kurarken veya yeniden kurarken kullanılacak kimlik doğrulama yöntemini belirtir."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/credentialsmethodtype/
---
## ExternalConnection.CredentialsMethodType property

Bağlantıyı kurarken (veya yeniden kurarken) kullanılacak kimlik doğrulama yöntemini belirtir.

```csharp
public CredentialsMethodType CredentialsMethodType { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using Aspose.Cells.Pivot;
    using System;

    public class ExternalConnectionPropertyCredentialsMethodTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Bir çalışma sayfası ekleyin ve dış bağlantı kurmak için bir pivot tablo oluşturun
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Cells["A1"].PutValue("Product");
                sheet.Cells["B1"].PutValue("Sales");
                sheet.Cells["A2"].PutValue("Apple");
                sheet.Cells["B2"].PutValue(1000);
                sheet.Cells["A3"].PutValue("Banana");
                sheet.Cells["B3"].PutValue(2000);

                // Dış bağlantısı olacak bir pivot tablo oluşturun
                int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
                Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

                // Pivot tablodan dış bağlantıyı alın
                ExternalConnection connection = pivotTable.GetSourceDataConnections()[0];

                // Mevcut CredentialsMethodType değerini göster
                Console.WriteLine("Initial CredentialsMethodType: " + connection.CredentialsMethodType);

                // Özelliği ayarlamayı gösterin (okuma-yazma olduğu için)
                connection.CredentialsMethodType = CredentialsMethodType.Stored;
                Console.WriteLine("Updated CredentialsMethodType: " + connection.CredentialsMethodType);

                // Başka bir değere ayarlayarak gösterin
                connection.CredentialsMethodType = CredentialsMethodType.Integrated;
                Console.WriteLine("Changed CredentialsMethodType: " + connection.CredentialsMethodType);

                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("CredentialsMethodTypeDemo.xlsx");
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

* enum [CredentialsMethodType](../../credentialsmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


