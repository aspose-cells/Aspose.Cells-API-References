---
title: "LowCodeSaveOptions.SaveFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptions-Eigenschaft. Gibt das Ausgabeformat zurück und legt es fest. Im Allgemeinen sind für bestimmte Prozesse im Low-Code‑Modus nur einige spezifische Formate zulässig. Bitte geben Sie das korrekte Format für den jeweiligen Prozess an, sonst kann ein unerwartetes Ergebnis oder sogar eine Ausnahme auftreten."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptions/saveformat/
---
## LowCodeSaveOptions.SaveFormat property

Liest und setzt das Speicherformat für die Ausgabe. Im Allgemeinen sind für einen bestimmten Prozess auf Low-Code-Weise nur einige spezifische Formate zulässig. Bitte geben Sie das korrekte Format für den jeweiligen Prozess an, sonst kann ein unerwartetes Ergebnis oder sogar eine Ausnahme auftreten.

```csharp
public virtual SaveFormat SaveFormat { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Initialisiere LowCodeSaveOptions mit verschiedenen Formaten
            LowCodeSaveOptions excelOptions = new LowCodeSaveOptions();
            LowCodeSaveOptions pdfOptions = new LowCodeSaveOptions();

            // Konfiguriere die Excel-Speicheroptionen
            excelOptions.SaveFormat = SaveFormat.Xlsx;
            excelOptions.OutputFile = "output_excel.xlsx";

            // PDF‑Speicheroptionen konfigurieren
            pdfOptions.SaveFormat = SaveFormat.Pdf;
            pdfOptions.OutputFile = "output_pdf.pdf";

            // Demonstriere das Speichern im Originalformat
            Console.WriteLine($"Saving as {excelOptions.SaveFormat}");
            workbook.Save(excelOptions.OutputFile, excelOptions.SaveFormat);

            // Demonstriere die Formatänderung und das erneute Speichern
            Console.WriteLine($"Changing format to {pdfOptions.SaveFormat}");
            Console.WriteLine($"Saving as {pdfOptions.SaveFormat}");
            workbook.Save(pdfOptions.OutputFile, pdfOptions.SaveFormat);

            Console.WriteLine("Files saved successfully with different formats.");
        }
    }
}
```

### Siehe auch

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


