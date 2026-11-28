---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. MS Excel'de dosya açılırken tüm bağlantıların yenilenip yenilenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

MS Excel'de dosya açılırken tüm bağlantıların yenilenip yenilenmeyeceğini gösterir.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfası koleksiyonuna eriş.
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Bazı örnek çalışma sayfaları ekleyin
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // IsRefreshAllConnections özelliğini ayarla
            worksheets.IsRefreshAllConnections = true;
            
            // IsRefreshAllConnections'ın mevcut değerini göster
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


