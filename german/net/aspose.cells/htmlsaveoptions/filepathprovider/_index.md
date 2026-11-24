---
title: "HtmlSaveOptions.FilePathProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions Eigenschaft. Ruft den IFilePathProvider ab oder legt ihn fest, um das Arbeitsblatt separat nach html zu exportieren"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/filepathprovider/
---
## HtmlSaveOptions.FilePathProvider property

Ruft den IFilePathProvider ab oder legt ihn fest, um das Arbeitsblatt separat nach HTML zu exportieren.

```csharp
public IFilePathProvider FilePathProvider { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFilePathProviderDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und füge einige Daten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Erstelle HtmlSaveOptions und setze den FilePathProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.FilePathProvider = new CustomFilePathProvider();

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("Workbook saved to HTML with custom file paths.");
        }
    }

    public class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Benutzerdefinierte Logik zum Erzeugen von Dateipfaden
            return $"custom_{sheetName}";
        }
    }
}
```

### Siehe auch

* interface [IFilePathProvider](../../ifilepathprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


