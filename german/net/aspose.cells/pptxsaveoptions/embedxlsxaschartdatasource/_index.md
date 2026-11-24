---
title: "PptxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PptxSaveOptions-Eigenschaft. Gibt an, ob eine xlsx-Datei als Datenquelle des Diagramms eingebettet wird."
type: docs
url: /de/net/aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/
---
## PptxSaveOptions.EmbedXlsxAsChartDataSource property

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
    using Aspose.Cells.Charts;
    using System;

    public class PptxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein Beispiel-Arbeitsblatt mit Diagrammdaten erstellen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Ein Diagramm hinzufügen, um die Wirkung der Eigenschaft zu demonstrieren
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Erstelle eine PptxSaveOptions-Instanz
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Den Standardwert von EmbedXlsxAsChartDataSource anzeigen
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Setze die Eigenschaft auf true, um ihre Verwendung zu demonstrieren
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Speichere die Arbeitsmappe als PPTX mit aktivierter Option
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with EmbedXlsxAsChartDataSource enabled");
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

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


