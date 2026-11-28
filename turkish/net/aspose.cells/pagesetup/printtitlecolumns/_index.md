---
title: "PageSetup.PrintTitleColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PageSetup özelliği. Her sayfanın sol tarafında tekrarlanacak hücreleri içeren sütunları temsil eder"
type: docs
url: /tr/net/aspose.cells/pagesetup/printtitlecolumns/
---
## PageSetup.PrintTitleColumns property

Her sayfanın sol tarafında tekrarlanacak hücreleri içeren sütunları temsil eder.

```csharp
public string PrintTitleColumns { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleColumnsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sayfa ayarına eriş
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Yazdırma başlık sütunlarını, her basılan sayfada A sütununu tekrarlayacak şekilde ayarla
            pageSetup.PrintTitleColumns = "$A:$A";
            
            // Etkiyi göstermek için A sütununa bazı veriler ekle
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Title Column - Row {i + 1}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PrintTitleColumnsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


