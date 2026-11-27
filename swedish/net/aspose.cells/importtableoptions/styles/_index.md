---
title: "ImportTableOptions.Styles"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Hämtar och anger stilarna för varje kolumn i tabellen"
type: docs
url: /sv/net/aspose.cells/importtableoptions/styles/
---
## ImportTableOptions.Styles property

Hämtar och anger stilarna för varje kolumn i tabellen.

```csharp
public Style[] Styles { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldatatabell
            DataTable dt = new DataTable();
            dt.Columns.Add("Product");
            dt.Columns.Add("Price");
            dt.Rows.Add("Apple", 1.50);
            dt.Rows.Add("Banana", 0.75);
            dt.Rows.Add("Orange", 1.20);

            try
            {
                // Skapa ImportTableOptions och ange Styles‑egenskap
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;

                // Skapa stilar för varje kolumn
                Style[] columnStyles = new Style[2];

                // Stil för Product‑kolumn (fet, blått teckensnitt)
                Style productStyle = workbook.CreateStyle();
                productStyle.Font.IsBold = true;
                productStyle.Font.Color = System.Drawing.Color.Blue;
                columnStyles[0] = productStyle;

                // Stil för Price‑kolumn (valutaformat, grönt teckensnitt)
                Style priceStyle = workbook.CreateStyle();
                priceStyle.Font.Color = System.Drawing.Color.Green;
                priceStyle.Number = 4; // Currency format
                columnStyles[1] = priceStyle;

                // Ställ in Styles‑egenskapen
                options.Styles = columnStyles;

                // Importera data med stilar
                worksheet.Cells.ImportData(dt, 0, 0, options);

                // Visa de tillämpade stilarna
                Console.WriteLine("Styles applied to columns:");
                Console.WriteLine($"Product column style: Bold={columnStyles[0].Font.IsBold}, Color={columnStyles[0].Font.Color.Name}");
                Console.WriteLine($"Price column style: NumberFormat={columnStyles[1].Number}, Color={columnStyles[1].Font.Color.Name}");

                // Spara arbetsboken
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

### Se även

* class [Style](../../style/)
* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


