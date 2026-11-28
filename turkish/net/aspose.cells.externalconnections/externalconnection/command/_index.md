---
title: "ExternalConnection.Command"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Dış kaynağa veri almak için veri sağlayıcı API'sine gönderilecek veritabanı komutunu içeren dize."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

Veri sağlayıcı API'sine dış kaynağa etkileşimde bulunarak veri almak için gönderilecek veritabanı komutunu içeren dize.

```csharp
public virtual string Command { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ve bazı örnek veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // Bir tablo aralığı oluşturun
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // Aralığı kaynak olarak kullanarak bir pivot tablo oluşturun
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // Dış bağlantıları alın
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Bağlantının Command özelliğini göster
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


