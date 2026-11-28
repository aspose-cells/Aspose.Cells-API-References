---
title: "ExternalConnection.SourceType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Dış bağlantı DataSource türünü alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

Harici bağlantının DataSource türünü alır veya ayarlar.

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertySourceTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekleyin ve bir pivot tablo oluşturun
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B3"].PutValue(2000);
            
            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B3", "C3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
            
            // Harici bağlantıyı al
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // SourceType özelliğini gösterin
            Console.WriteLine("Connection Source Type: " + conn.SourceType);
            
            // Bağlantı özelliklerini değiştirin
            conn.Name = "TestConnection";
            conn.SourceType = ConnectionDataSourceType.OLEDBDataModel;
            
            // Değiştirilen özellikleri çıktı olarak verin
            Console.WriteLine("Modified Connection Name: " + conn.Name);
            Console.WriteLine("Modified Source Type: " + conn.SourceType);
        }
    }
}
```

### Ayrıca Bakınız

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


