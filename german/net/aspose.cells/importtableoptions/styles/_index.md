---
title: "ImportTableOptions.Styles"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Ruft die Stile für jede Spalte der Tabelle ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

Liest und legt die Stile für jede Spalte der Tabelle fest

```csharp
public Style[] Styles { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyStylesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieltabelle erstellen
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // ImportTableOptions erstellen und die Styles-Eigenschaft festlegen
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // Stile für jede Spalte erstellen
                Style[] columnStyles = new Style[2];

                // Stil für die Spalte Produkt (fett, blaue Schrift)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Stil für die Spalte Preis (Währungsformat, grüne Schrift)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // Die Styles-Eigenschaft festlegen
                options.Styles = columnStyles;

                // Daten mit Stilen importieren
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // Angewendete Stile anzeigen
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // Speichere die Arbeitsmappe
                workbook.Save("StylesDemo.xlsx");
                Console.WriteLine("Workbook saved with styled data.");
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

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


