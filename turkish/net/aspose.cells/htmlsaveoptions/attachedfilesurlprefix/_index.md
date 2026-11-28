---
title: "HtmlSaveOptions.AttachedFilesUrlPrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca HTML akışına kaydetmek için kullanılır."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/attachedfilesurlprefix/
---
## HtmlSaveOptions.AttachedFilesUrlPrefix property

HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. Yalnızca HTML akışına kaydetme için.

```csharp
public string AttachedFilesUrlPrefix { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesUrlPrefixDemo
    {
        public static void Run()
        {
            // Örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // AttachedFilesUrlPrefix ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";

            // Çalışma kitabını HTML seçenekleriyle kaydet
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with AttachedFilesUrlPrefix: " + saveOptions.AttachedFilesUrlPrefix);
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


