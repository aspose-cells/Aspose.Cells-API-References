---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Gibt an, ob die Spaltenausrichtung für erzeugte Markdown-Tabellen aktiviert ist. Wenn aktiviert, werden die Spalten durch Auffüllen des Zelleninhalts mit dem angegebenen Zeichen, typischerweise einem Leerzeichen, ausgerichtet. Setzen Sie den Wert auf 0, um die Spaltenausrichtung zu deaktivieren (Standard)."
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Gibt an, ob die Spaltenausrichtung für erzeugte Markdown-Tabellen aktiviert ist. Wenn aktiviert, werden die Spalten durch Auffüllen des Zelleninhalts mit dem angegebenen Zeichen (typischerweise ' ' für Leerzeichen) ausgerichtet. Setzen Sie es auf '\0', um die Spaltenausrichtung zu deaktivieren (Standard).

```csharp
public char AlignColumnPadding { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu, um die Spaltenausrichtung zu demonstrieren
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // Erstelle eine MarkdownSaveOptions-Instanz.
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Zeigen Sie den Standardwert von AlignColumnPadding an
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Setzen Sie AlignColumnPadding auf das Leerzeichen für die Spaltenausrichtung
                saveOptions.AlignColumnPadding = ' ';

                // Zeigen Sie den aktualisierten Wert an
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Speichern Sie die Arbeitsmappe als Markdown mit Spaltenausrichtung
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


