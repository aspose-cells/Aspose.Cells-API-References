---
title: "Workbook.HasExernalLinks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bu çalışma kitabının diğer veri kaynaklarına dış bağlantılar içerip içermediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Bu çalışma kitabının diğer veri kaynaklarına dış bağlantılar içerip içermediğini gösterir.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Dönüş Değeri

Bu çalışma kitabının diğer veri kaynaklarına dış bağlantılar içerip içermediği.

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, bu çalışma kitabında dış bağlantıların olup olmadığını kontrol etmek için ExternalLinkCollection.Count kullanın. Bu yöntem, Aralık 2021'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // Dış bağlantılar içeren bir çalışma kitabı oluşturun
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // Bir dış bağlantı ekleyin
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // Çalışma kitabının dış bağlantıları olup olmadığını kontrol edin
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


