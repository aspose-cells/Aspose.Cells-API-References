---
title: "Sınıf ExternalLinkCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalLinkCollection sınıfı. Bir çalışma kitabındaki dış bağlantılar koleksiyonunu temsil eder"
type: docs
url: /tr/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

Çalışma kitabındaki harici bağlantılar koleksiyonunu temsil eder.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Koleksiyonda gerçekte bulunan öğe sayısını alır. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Belirtilen indeksteki [`ExternalLink`](../externallink/) öğesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Bir dış bağlantı ekler. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Bir dış bağlantı ekle . |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Tüm dış bağlantıları kaldırır. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Tüm dış bağlantıları kaldırır. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Bu koleksiyon içinde yineleme yapan bir enumerator al. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Belirtilen dış bağlantıyı çalışma kitabından kaldırır. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Belirtilen dış bağlantıyı çalışma kitabından kaldırır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // Dış bağlantılar içeren bir dosya aç
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // Dış bağlantılar koleksiyonunu al
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // Dış bağlantıların sayısını göster
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // Dış bağlantılar arasında yineleme yap ve veri kaynaklarını göster
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // Yeni bir dış bağlantı ekle
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // İlk dış bağlantının veri kaynağını değiştir
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // Tüm dış bağlantıları temizle
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // Harici bağlantıları temizledikten sonra çalışma kitabını kaydedin
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


