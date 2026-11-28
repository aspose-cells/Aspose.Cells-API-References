---
title: "AutoFitterOptions.IgnoreHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFitterOptions özelliği. Gizli satırları/sütunları yok sayar"
type: docs
url: /tr/net/aspose.cells/autofitteroptions/ignorehidden/
---
## AutoFitterOptions.IgnoreHidden property

Gizli satırları/sütunları yok sayar.

```csharp
public bool IgnoreHidden { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyIgnoreHiddenDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek verileri ayarlayın ve satırları biçimlendirin
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["A2"].PutValue("Another test string");
            
            // Satır 1'i gizle
            worksheet.Cells.Rows[1].IsHidden = true;

            // IgnoreHidden true olarak ayarlanmış AutoFitterOptions oluşturun
            AutoFitterOptions options = new AutoFitterOptions
            {
                IgnoreHidden = true,
                AutoFitMergedCells = false,
                OnlyAuto = false
            };

            // Gizli satırları yok sayarken satırları otomatik sığdırın
            worksheet.AutoFitRows(options);

            // Satır yüksekliklerini çıktı olarak verin
            Console.WriteLine("Row 0 height: " + worksheet.Cells.GetRowHeight(0));
            Console.WriteLine("Row 1 height: " + worksheet.Cells.GetRowHeight(1));
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


