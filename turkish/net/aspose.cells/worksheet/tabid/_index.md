---
title: "Worksheet.TabId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Sayfa için dahili tanımlayıcıyı belirtir"
type: docs
url: /tr/net/aspose.cells/worksheet/tabid/
---
## Worksheet.TabId property

Sayfa için iç tanımlayıcıyı belirtir.

```csharp
public int TabId { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // TabId özelliğini ayarla
            worksheet.TabId = 107;
            
            // Çalışma kitabını kaydedin
            string outputPath = "output.xlsb";
            workbook.Save(outputPath);
            
            // Kaydedilmiş çalışma kitabını yükle ve TabId'yi doğrula
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // TabId değerini göster
            Console.WriteLine("Worksheet TabId: " + loadedWorksheet.TabId);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


