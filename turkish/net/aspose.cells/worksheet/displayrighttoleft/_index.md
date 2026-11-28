---
title: "Worksheet.DisplayRightToLeft"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini belirtir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola görüntülenip görüntülenmediğini gösterir. Varsayılan değer false'tur.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayRightToLeftDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sağdan sola görüntülemeyi ayarlayın
            worksheet.DisplayRightToLeft = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.ods");
            
            // Ayarı doğrulamak için çalışma kitabını yeniden yükleyin
            Workbook loadedWorkbook = new Workbook("output.ods");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


