---
title: "Worksheet.ErrorCheckOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Belirli aralıklara uygulanan hata kontrol ayarını alır"
type: docs
url: /tr/net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

Belirli aralıklara uygulanan hata kontrol ayarını alır.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyErrorCheckOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hata kontrol seçeneklerini etkinleştirin
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            ErrorCheckOption option = options[0]; // Properly access first option using indexer
            option.SetErrorCheck(ErrorCheckType.TextDate, true);
            option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
            
            // Seçenek için aralık sayısını alın
            int rangeCount = option.GetCountOfRange();
            Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


