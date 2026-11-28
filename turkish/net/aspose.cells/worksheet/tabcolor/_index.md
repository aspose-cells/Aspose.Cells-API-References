---
title: "Worksheet.TabColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfası sekmesinin rengini temsil eder"
type: docs
url: /tr/net/aspose.cells/worksheet/tabcolor/
---
## Worksheet.TabColor property

Çalışma sayfası sekme rengini temsil eder.

```csharp
public Color TabColor { get; set; }
```

### Açıklamalar

Bu özellik yalnızca ExcelXP (Excel2002) ve sonraki sürümlerde desteklenir. Dosyayı Excel97 veya Excel2000 formatında kaydederseniz, atlanacaktır.

### Örnekler

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTabColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sekme rengini kırmızı olarak ayarla
            worksheet.TabColor = Color.Red;
            Console.WriteLine("Tab color set to: " + worksheet.TabColor);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Sekme rengini temizle
            worksheet.TabColor = Color.Empty;
            Console.WriteLine("Tab color cleared: " + worksheet.TabColor.IsEmpty);
            
            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("output_modified.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


