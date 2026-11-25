---
title: "ImportTableOptions.Styles"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Ottiene e imposta gli stili per ogni colonna della tabella"
type: docs
url: /it/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

Ottiene e imposta gli stili per ogni colonna della tabella.

```csharp
public Style[] Styles { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una tabella di dati di esempio
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // Crea ImportTableOptions e imposta la proprietà Styles
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // Crea stili per ogni colonna
                Style[] columnStyles = new Style[2];

                // Stile per la colonna Prodotto (grassetto, carattere blu)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Stile per la colonna Prezzo (formato valuta, carattere verde)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // Imposta la proprietà Styles
                options.Styles = columnStyles;

                // Importa dati con stili
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // Visualizza gli stili applicati
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // Salva la cartella di lavoro
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

### Vedi anche

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


