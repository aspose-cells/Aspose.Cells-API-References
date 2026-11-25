---
title: "FontSettingCollection.HtmlString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSettingCollection. Ottiene e imposta la stringa html che contiene dati e alcuni formati in questa forma"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/htmlstring/
---
## FontSettingCollection.HtmlString property

Ottiene e imposta la stringa html che contiene dati e alcuni formati in questa forma.

```csharp
public string HtmlString { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 300, 100);
            var fontSettingCollection = textBox.TextBody;

            // Imposta il testo iniziale con formattazione HTML
            string initialHtml = "<b>Bold Text</b> and <i>Italic Text</i>";
            fontSettingCollection.HtmlString = initialHtml;

            // Visualizza la stringa HTML corrente
            Console.WriteLine("Initial HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text: " + fontSettingCollection.Text);

            // Modifica la stringa HTML per aggiungere ulteriore formattazione
            string modifiedHtml = "<font color='red'>Red Text</font> and <u>Underlined Text</u>";
            fontSettingCollection.HtmlString = modifiedHtml;

            // Visualizza i valori modificati
            Console.WriteLine("\nModified HtmlString value: " + fontSettingCollection.HtmlString);
            Console.WriteLine("Rendered Text after modification: " + fontSettingCollection.Text);

            // Aggiungi una cella con testo formattato in HTML
            var cell = worksheet.Cells["A1"];
            cell.HtmlString = "<b>Cell HTML</b> <i>Formatted</i> <font color='blue'>Text</font>";

            // Salva la cartella di lavoro per mostrare sia la formattazione HTML della casella di testo che della cella
            workbook.Save("FontSettingCollectionHtmlStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


