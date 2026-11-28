---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HighlightChangesOptions yapıcı. Paylaşılan Excel dosyalarındaki revizyonları veya değişiklikleri vurgulama seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Paylaşılan Excel dosyalarının revizyonlarını veya değişikliklerini vurgulama seçeneklerini temsil eder.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| highlightOnScreen | Boolean | Ekranda değişiklikleri vurgulayıp vurgulamadığını gösterir. |
| listOnNewSheet | Boolean | Değişikliklerin yeni bir çalışma sayfasına listelenip listelenmeyeceğini gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Boolean parametrelerle HighlightChangesOptions oluştur
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // Değişiklik izlemeyi simüle et (normalde gerçek revizyonlarınız olur)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


