---
title: "DisplayUnitLabel.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DisplayUnitLabel. Ottiene un oggetto Font del ChartFrame specificato"
type: docs
url: /it/net/aspose.cells.charts/displayunitlabel/font/
---
## DisplayUnitLabel.Font property

Restituisce un oggetto `Font` dell'oggetto ChartFrame specificato.

```csharp
public override Font Font { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitLabelPropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            worksheet.Cells["A5"].PutValue(5000);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Imposta le unità di visualizzazione per l'asse dei valori
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.DisplayUnitLabel.Text = "Thousands";

            // Ottieni l'istanza di DisplayUnitLabel
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Visualizza le proprietà attuali del font
            Font currentFont = displayUnitLabel.Font;
            Console.WriteLine("Current Font Properties:");
            Console.WriteLine($"Name: {currentFont.Name}");
            Console.WriteLine($"Size: {currentFont.Size}");
            Console.WriteLine($"Color: {currentFont.Color}");
            Console.WriteLine($"Bold: {currentFont.IsBold}");
            Console.WriteLine($"Italic: {currentFont.IsItalic}");

            // Crea un nuovo stile di carattere e applicalo all'etichetta dell'unità di visualizzazione
            // Nota: Poiché Font è di sola lettura, modifichiamo le sue proprietà direttamente
            currentFont.Name = "Arial";
            currentFont.Size = 12;
            currentFont.Color = System.Drawing.Color.Red;
            currentFont.IsBold = true;
            currentFont.IsItalic = false;
            currentFont.Underline = FontUnderlineType.Single;

            // Salva la cartella di lavoro per vedere le modifiche
            workbook.Save("DisplayUnitLabelFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


