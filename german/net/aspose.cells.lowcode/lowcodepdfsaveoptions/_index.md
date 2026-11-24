---
title: "Klasse LowCodePdfSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodePdfSaveOptions Klasse. Optionen zum Speichern von PDF auf Low‑Code‑Weise"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodepdfsaveoptions/
---
## LowCodePdfSaveOptions class

Optionen zum Speichern von PDF in Low‑Code‑Manier.

```csharp
public class LowCodePdfSaveOptions : LowCodeSaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodePdfSaveOptions](lowcodepdfsaveoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | Liest und schreibt die Datei (mit Pfad, falls erforderlich) zum Speichern der erzeugten Daten. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null oder ein leerer String ist, wird [`OutputStream`](../lowcodesaveoptions/outputstream/) ignoriert. (Geerbt von [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | Liest und schreibt den Stream, in den die erzeugten Daten geschrieben werden. Beim Setzen dieser Eigenschaft mit einem Wert, der nicht null ist, wird [`OutputFile`](../lowcodesaveoptions/outputfile/) ignoriert. (Geerbt von [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [PdfOptions](../../aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/) { get; set; } | Die Optionen zum Speichern der PDF‑Datei. |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodepdfsaveoptions/saveformat/) { get; set; } | Das Speicherformat für die Ausgabe. Beim Konvertieren zu PDF kann nur PDF verwendet werden. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class LowCodeClassLowCodePdfSaveOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Compliance = PdfCompliance.PdfA1b;

            // Erstelle Low-Code-PDF-Speicheroptionen
            LowCodePdfSaveOptions lowCodePdfOptions = new LowCodePdfSaveOptions()
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfOptions
            };

            // Speichere mit Low-Code-Optionen
            workbook.Save(lowCodePdfOptions.OutputFile, lowCodePdfOptions.PdfOptions);

            Console.WriteLine("File saved successfully with LowCodePdfSaveOptions");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


