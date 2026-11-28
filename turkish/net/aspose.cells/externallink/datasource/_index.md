---
title: "ExternalLink.DataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalLink özelliği. Harici bağlantının veri kaynağını temsil eder"
type: docs
url: /tr/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Harici bağlantının veri kaynağını temsil eder.

```csharp
public string DataSource { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Başka bir çalışma kitabına harici bir bağlantı oluşturun
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Harici bağlantıları kontrol etmek için kaydedilmiş çalışma kitabını yükleyin
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Harici bağlantının DataSource özelliğine erişin
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


