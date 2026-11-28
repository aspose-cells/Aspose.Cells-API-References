---
title: "Worksheet.TransitionEvaluation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Geçiş Formül Değerlendirmesi Lotus uyumluluk seçeneğinin etkin olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Geçiş Formül Değerlendirmesi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını gösterir.

```csharp
public bool TransitionEvaluation { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // TransitionEvaluation özelliğini ayarla
            worksheet.TransitionEvaluation = true;
            
            // Özellik değerini göster
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyerek özelliği doğrulayın
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


