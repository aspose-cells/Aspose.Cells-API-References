---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen.

```csharp
public bool CalculateFormula { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit Formeln hinzufügen
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // Erstelle eine MarkdownSaveOptions-Instanz.
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Den Standardwert von CalculateFormula anzeigen
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Setze CalculateFormula auf true, um Formeln vor dem Speichern zu berechnen
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Speichere die Arbeitsmappe mit aktivierter Formelberechnung
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Setze CalculateFormula auf false, um Formeln unverändert zu speichern
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Speichere die Arbeitsmappe mit deaktivierter Formelberechnung
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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


