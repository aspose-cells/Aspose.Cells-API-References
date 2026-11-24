---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions-Eigenschaft. Gibt an, ob leere Zeilen im Arbeitsblatt beim Exportieren nach Markdown als Tabellentrenner behandelt werden sollen. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrennzeichen behandelt werden sollen. Der Standardwert ist false.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit leeren Zeilen hinzufügen, um die Tabellenteilung zu demonstrieren
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // Füge eine leere Zeile hinzu (Zeile 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // Erstelle eine MarkdownSaveOptions-Instanz.
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Den Standardwert von SplitTablesByBlankRow anzeigen
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Setze SplitTablesByBlankRow auf true, um Tabellen anhand leerer Zeilen zu teilen
                saveOptions.SplitTablesByBlankRow = true;

                // Zeigen Sie den aktualisierten Wert an
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Speichere die Arbeitsmappe als Markdown mit aktivierter Tabellenteilung
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
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


