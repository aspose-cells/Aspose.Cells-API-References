---
title: "ExternalConnection.SSOId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Ara bir spreadsheetML sunucusu ile dış veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

Ara bir spreadsheetML sunucusu ile harici veri kaynağı arasında kimlik doğrulama için kullanılan Tek Oturum Açma (SSO) tanımlayıcısı.

```csharp
public string SSOId { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySSOIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin
                ExternalConnection connection = workbook.DataConnections[0];
                
                // İlk SSOId değerini gösterin (yeni bağlantı için muhtemelen null)
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // Yeni bir SSOId değeri ayarlayın (çünkü okunabilir-yazılabilir)
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // SSOId'yi temizleyin
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("SSOIdDemo.xlsx");
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


