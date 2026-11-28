---
title: "HtmlSaveOptions.AttachedFilesDirectory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Ekli dosyaların kaydedileceği dizin. Yalnızca html akışına kaydetmek için."
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/attachedfilesdirectory/
---
## HtmlSaveOptions.AttachedFilesDirectory property

Ekli dosyaların kaydedileceği dizin. Yalnızca HTML akışına kaydetme için.

```csharp
public string AttachedFilesDirectory { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Demonstrasyon için geçici bir dizin oluşturun
            string tempDir = Path.Combine(Path.GetTempPath(), "AsposeAttachedFilesDemo");
            Directory.CreateDirectory(tempDir);

            try
            {
                // Örnek bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Hello World");

                // AttachedFilesDirectory ile HTML kaydetme seçeneklerini ayarlayın
                HtmlSaveOptions options = new HtmlSaveOptions();
                options.AttachedFilesDirectory = tempDir;

                // Çalışma kitabını HTML olarak kaydet
                string outputPath = Path.Combine(tempDir, "output.html");
                workbook.Save(outputPath, options);

                // Ekli dosyaların oluşturulduğunu doğrulayın
                Console.WriteLine("HTML saved with attached files in: " + tempDir);
                Console.WriteLine("Attached files exist: " + 
                    File.Exists(Path.Combine(tempDir, "sheet001.htm")));
            }
            finally
            {
                // Temizle
                Directory.Delete(tempDir, true);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


