---
title: "Sınıf ExternalLink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalLink sınıfı. Bir çalışma kitabındaki harici bağlantıyı temsil eder"
type: docs
url: /tr/net/aspose.cells/externallink/
---
## ExternalLink class

Çalışma kitabındaki harici bir bağlantıyı temsil eder.

```csharp
public class ExternalLink
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DataSource](../../aspose.cells/externallink/datasource/) { get; set; } | Harici bağlantının veri kaynağını temsil eder. |
| [IsReferred](../../aspose.cells/externallink/isreferred/) { get; } | Bu harici bağlantının diğerleri tarafından referans alınıp alınmadığını gösterir. |
| [IsVisible](../../aspose.cells/externallink/isvisible/) { get; } | Bu harici bağlantının MS Excel'de görünür olup olmadığını gösterir. |
| [OriginalDataSource](../../aspose.cells/externallink/originaldatasource/) { get; set; } | Harici bağlantının depolanmış veri kaynağını temsil eder. |
| [PathType](../../aspose.cells/externallink/pathtype/) { get; } | Bu harici bağlantının yol türünü alın |
| [Type](../../aspose.cells/externallink/type/) { get; } | Harici bağlantının türünü alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddExternalName](../../aspose.cells/externallink/addexternalname/)(string, string) | Harici bir ad ekler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkDemo
    {
        public static void ExternalLinkExample()
        {
            // Dış bağlantılar içeren bir dosya aç
            Workbook workbook = new Workbook("UpdatedExternalLinkExample_original.xlsx");

            // Dış Bağlantıyı Al 
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];

            // Harici bağlantının özelliklerini göster
            Console.WriteLine("External Link Type: " + externalLink.Type);
            Console.WriteLine("Path Type: " + externalLink.PathType);
            Console.WriteLine("Original Data Source: " + externalLink.OriginalDataSource);
            Console.WriteLine("Data Source: " + externalLink.DataSource);
            Console.WriteLine("Is Referred: " + externalLink.IsReferred);
            Console.WriteLine("Is Visible: " + externalLink.IsVisible);

            // Dış Bağlantının Veri Kaynağını Değiştir
            externalLink.DataSource = "d:\\linktest.xls";

            // Harici bağlantıya bir harici ad ekle
            externalLink.AddExternalName("ExternalName", "Sheet1!A1");

            // Çalışma kitabını kaydedin
            workbook.Save("UpdatedExternalLinkExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


