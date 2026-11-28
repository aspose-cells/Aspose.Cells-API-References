---
title: "WorksheetCollection.ExternalLinks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Bir çalışma kitabındaki harici bağlantıları temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Bir çalışma kitabındaki harici bağlantıları temsil eder.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // Harici bağlantılı bir kaynak çalışma kitabı oluştur
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // Bir hedef çalışma kitabı oluştur
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // Harici bağlantı veri kaynağını ayarla
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // Çalışma kitabını kaydedin
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // Temizle
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


