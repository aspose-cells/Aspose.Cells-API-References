---
title: "ExternalLink.IsVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLink özelliği. Bu harici bağlantının MS Excel'de görünür olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Bu harici bağlantının MS Excel'de görünür olup olmadığını gösterir.

```csharp
public bool IsVisible { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Dış bağlantılar içeren bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // Harici bağlantı kaynağı olarak kullanılacak yeni bir çalışma kitabı oluşturun
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // Harici bir bağlantı referansı ekle
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // Harici bağlantıları kontrol edin (formüller yüklenirken otomatik olarak oluşturulacaklardır)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // Mevcut dosyayı yüklemeyi göstermek için başka bir çalışma kitabı oluşturun
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // Harici bağlantıları göstermek için kaydedin ve yeniden yükleyin
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Yüklenmiş çalışma kitabındaki harici bağlantıları kontrol edin
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


