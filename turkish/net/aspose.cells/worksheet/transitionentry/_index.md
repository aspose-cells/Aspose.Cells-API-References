---
title: "Worksheet.TransitionEntry"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Transition Formula Entry Lotus uyumluluk seçeneğinin etkin olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/worksheet/transitionentry/
---
## Worksheet.TransitionEntry property

Geçiş Formül Girişi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını gösterir.

```csharp
public bool TransitionEntry { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEntryDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // TransitionEntry özelliğini ayarla
            worksheet.TransitionEntry = true;
            
            // TransitionEntry değerini göster
            Console.WriteLine("TransitionEntry: " + worksheet.TransitionEntry);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyerek özelliği doğrulayın
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Yüklenen TransitionEntry değerini göster
            Console.WriteLine("Loaded TransitionEntry: " + loadedWorksheet.TransitionEntry);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


