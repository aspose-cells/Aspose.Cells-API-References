---
title: "HtmlSaveOptions.ExportWorksheetCSSSeparately"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Çalışma sayfası css'sinin ayrı olarak dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/exportworksheetcssseparately/
---
## HtmlSaveOptions.ExportWorksheetCSSSeparately property

Çalışma sayfası CSS'inin ayrı ayrı dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetCSSSeparatelyDemo
    {
        public static void Run()
        {
            // Test verileriyle örnek bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // ExportWorksheetCSSSeparately ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportWorksheetCSSSeparately = true;
            
            // Çalışma kitabını HTML olarak kaydet
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with separate CSS saved to: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


