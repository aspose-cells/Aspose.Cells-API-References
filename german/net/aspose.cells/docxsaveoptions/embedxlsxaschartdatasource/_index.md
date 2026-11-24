---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DocxSaveOptions‑Eigenschaft. Gibt an, ob eine xlsx‑Datei als Datenquelle des Diagramms eingebettet wird"
type: docs
url: /de/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

Gibt an, ob eine xlsx‑Datei als Datenquelle des Diagramms eingebettet wird.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Hinweise

Der Standardwert ist true.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // DocxSaveOptions initialisieren
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Zeigen Sie den Standardwert der Eigenschaft EmbedXlsxAsChartDataSource an
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Setzen Sie EmbedXlsxAsChartDataSource auf true, um die Verwendung zu demonstrieren
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Speichern Sie die Arbeitsmappe als DOCX mit den konfigurierten Optionen
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


