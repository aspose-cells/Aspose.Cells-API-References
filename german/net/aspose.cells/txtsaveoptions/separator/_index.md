---
title: "TxtSaveOptions.Separator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Liest und setzt das Zeichen Delimiter der Textdatei"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Liest und setzt das Zeichen‑Trennzeichen der Textdatei.

```csharp
public char Separator { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // TXT-Speicheroptionen mit Komma‑Trennzeichen konfigurieren
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.Separator = ',';
            txtSaveOptions.Encoding = System.Text.Encoding.UTF8;

            // Arbeitsmappe als CSV mit Komma‑Trennzeichen speichern
            string outputPath = "output.csv";
            workbook.Save(outputPath, txtSaveOptions);

            // Gespeicherten Dateinhalt anzeigen
            Console.WriteLine("File saved with comma separator:");
            Console.WriteLine(File.ReadAllText(outputPath));
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


