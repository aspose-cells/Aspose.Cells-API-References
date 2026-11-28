---
title: "Worksheet.Hyperlinks"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. HyperlinkCollection koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Alır [`HyperlinkCollection`](../../hyperlinkcollection/) koleksiyonunu.

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir hiperlink ekleyin
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // Çalışma kitabını kaydedin
            workbook.Save("HyperlinksDemo.xlsx");
            
            // Hiperlinki doğrulamak için kaydedilmiş çalışma kitabını yükleyin
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Köprü adresini göster
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### Ayrıca Bakınız

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


