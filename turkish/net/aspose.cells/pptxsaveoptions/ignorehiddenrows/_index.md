---
title: "PptxSaveOptions.IgnoreHiddenRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PptxSaveOptions özelliği. Excel'den PowerPoint'e dönüştürürken gizli satırların göz ardı edilip edilmediğini gösterir."
type: docs
url: /tr/net/aspose.cells/pptxsaveoptions/ignorehiddenrows/
---
## PptxSaveOptions.IgnoreHiddenRows property

Excel'den PowerPoint'e dönüştürürken gizli satırların göz ardı edilip edilmeyeceğini gösterir.

```csharp
public bool IgnoreHiddenRows { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyIgnoreHiddenRowsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin ve bazı satırları gizleyin
            worksheet.Cells["A1"].PutValue("Visible Row 1");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row 2");
            
            // Satır 2'yi gizle
            worksheet.Cells.Rows[1].IsHidden = true;

            // IgnoreHiddenRows ile PPTX kaydetme seçeneklerini ayarlayın
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.IgnoreHiddenRows = true;
            
            // PPTX olarak kaydet
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("PPTX saved with hidden rows ignored.");
        }
    }
}
```

### Ayrıca Bakınız

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


