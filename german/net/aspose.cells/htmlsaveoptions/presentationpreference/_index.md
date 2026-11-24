---
title: "HtmlSaveOptions.PresentationPreference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob HTML- oder MHT-Dateien als Präsentationspräferenz gelten. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert auf true"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/presentationpreference/
---
## HtmlSaveOptions.PresentationPreference property

Gibt an, ob HTML‑ oder MHT‑Datei die Präsentationspräferenz ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert bitte auf true.

```csharp
public bool PresentationPreference { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyPresentationPreferenceDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Presentation Preference Test");
            worksheet.Cells["B1"].PutValue(123.45);
            worksheet.Cells["A2"].PutValue(DateTime.Now);

            // Setzen Sie HTML-Speicheroptionen mit PresentationPreference
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.PresentationPreference = true;
            options.IsFullPathLink = false;

            // In einen Memory-Stream speichern zur Demonstration
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                Console.WriteLine("Workbook saved with PresentationPreference=true");
            }
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


