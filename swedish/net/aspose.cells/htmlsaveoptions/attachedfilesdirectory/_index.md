---
title: "HtmlSaveOptions.AttachedFilesDirectory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions property. Katalogen där de bifogade filerna kommer att sparas. Endast för sparande till HTML‑ström."
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/attachedfilesdirectory/
---
## HtmlSaveOptions.AttachedFilesDirectory property

Den katalog som de bifogade filerna kommer att sparas i. Endast för att spara till html‑ström.

```csharp
public string AttachedFilesDirectory { get; set; }
```

### Exempel

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
            // Skapa en temporär katalog för demonstration
            string tempDir = Path.Combine(Path.GetTempPath(), "AsposeAttachedFilesDemo");
            Directory.CreateDirectory(tempDir);

            try
            {
                // Skapa en exempelarbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Hello World");

                // Ställ in HTML‑sparalternativ med AttachedFilesDirectory
                HtmlSaveOptions options = new HtmlSaveOptions();
                options.AttachedFilesDirectory = tempDir;

                // Spara arbetsboken som HTML
                string outputPath = Path.Combine(tempDir, "output.html");
                workbook.Save(outputPath, options);

                // Verifiera att de bifogade filerna skapades
                Console.WriteLine("HTML saved with attached files in: " + tempDir);
                Console.WriteLine("Attached files exist: " + 
                    File.Exists(Path.Combine(tempDir, "sheet001.htm")));
            }
            finally
            {
                // Rensa upp
                Directory.Delete(tempDir, true);
            }
        }
    }
}
```

### Se även

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


