---
title: "Enum GridlineType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridlineType enum. Izgara çizgi türlerini sıralar."
type: docs
url: /tr/net/aspose.cells/gridlinetype/
---
## GridlineType enumeration

Izgara çizgi türünü sıralar.

```csharp
public enum GridlineType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Dotted | `0` | Noktalı çizgiyi temsil eder. |
| Hair | `1` | İnce çizgiyi temsil eder. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassGridlineTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kaydetme seçeneklerini oluşturun ve ızgara çizgi türünü ayarlayın.
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.GridlineType = GridlineType.Dotted;
            
            // Izgara çizgileri görmek için bazı örnek veriler ekleyin.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            // Çalışma kitabını kaydetme seçenekleriyle kaydedin.
            workbook.Save("GridlineTypeDemo.docx", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


