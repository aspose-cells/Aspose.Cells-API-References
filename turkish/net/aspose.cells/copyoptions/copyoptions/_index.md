---
title: "CopyOptions.CopyOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CopyOptions yapıcı. CopyOptions yapıcı"
type: docs
url: /tr/net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

CopyOptions yapıcı.

```csharp
public CopyOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle ve ilk çalışma sayfasını al
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            
            // Kaynak sayfaya örnek veri ekle
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["A2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue(200);
            sourceSheet.Cells["A4"].PutValue(300);
            
            // CopyOptions'ı yapıcı kullanarak oluştur
            CopyOptions options = new CopyOptions();
            options.ReferToDestinationSheet = true;
            
            // Satırları seçeneklerle kopyala
            destSheet.Cells.CopyRows(sourceSheet.Cells, 0, 0, sourceSheet.Cells.MaxDisplayRange.RowCount, options);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CopyOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


