---
title: "Worksheet.Split"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Pencereyi böler"
type: docs
url: /tr/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Pencereyi böler.

```csharp
public void Split()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bölmeyi göstermek için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // Çalışma sayfasını böl (parametre gerekmez)
            worksheet.Split();
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


