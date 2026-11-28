---
title: "JsonSaveOptions.ExportHyperlinkType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "JsonSaveOptions özelliği. JSON'a hiperlink dışa aktarma türünü temsil eder"
type: docs
url: /tr/net/aspose.cells/jsonsaveoptions/exporthyperlinktype/
---
## JsonSaveOptions.ExportHyperlinkType property

JSON'a hiperlink dışa aktarma türünü temsil eder.

```csharp
public JsonExportHyperlinkType ExportHyperlinkType { get; set; }
```

### Açıklamalar

Varsayılan değer DisplayString'dir;

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Json;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportHyperlinkTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine bir köprü ekleyin
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // JSON için dışa aktarma seçeneklerini ayarla
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.ExportHyperlinkType = JsonExportHyperlinkType.HtmlString;
            
            // Çalışma kitabını JSON'a kaydet
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            // Çıktının hiperlink içerdiğini doğrula
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine("JSON content contains hyperlink: " + 
                jsonContent.Contains("https://www.aspose.com"));
        }
    }
}
```

### Ayrıca Bakınız

* enum [JsonExportHyperlinkType](../../../aspose.cells.json/jsonexporthyperlinktype/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


