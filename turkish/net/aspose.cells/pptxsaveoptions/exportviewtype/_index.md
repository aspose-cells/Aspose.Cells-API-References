---
title: "PptxSaveOptions.ExportViewType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PptxSaveOptions özelliği. PowerPoint'e dışa aktarırken görüntüleme türünü alır ve ayarlar. Varsayılan dışa aktarma türü, yazdırma gibi çalışır."
type: docs
url: /tr/net/aspose.cells/pptxsaveoptions/exportviewtype/
---
## PptxSaveOptions.ExportViewType property

PowerPoint'e dışa aktarırken görüntüleme tipini alır ve ayarlar. Varsayılan dışa aktarma tipi yazdırma gibi çalışır.

```csharp
public SlideViewType ExportViewType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class PptxSaveOptionsPropertyExportViewTypeDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // ExportViewType ile PPTX kaydetme seçeneklerini ayarlayın
            PptxSaveOptions saveOptions = new PptxSaveOptions();
            saveOptions.ExportViewType = SlideViewType.View;
            
            // Çalışma kitabını PPTX olarak kaydedin
            workbook.Save("output.pptx", saveOptions);
            
            Console.WriteLine("Workbook saved as PPTX with ExportViewType set to View");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SlideViewType](../../../aspose.cells.slides/slideviewtype/)
* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


