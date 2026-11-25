---
title: "FontSettingCollection.Text"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSettingCollection. Ottiene e imposta il testo della forma"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/text/
---
## FontSettingCollection.Text property

Ottiene e imposta il testo della forma.

```csharp
public string Text { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionPropertyTextDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            try
            {
                // Imposta il testo iniziale
                fontSettingCollection.Text = "Initial Text Value";
                Console.WriteLine("Initial Text value: " + fontSettingCollection.Text);

                // Modifica il testo
                fontSettingCollection.Text = "Modified Text Value";
                Console.WriteLine("Modified Text value: " + fontSettingCollection.Text);

                // Dimostra l'aggiunta di testo
                fontSettingCollection.AppendText(" (Appended)");
                Console.WriteLine("After AppendText: " + fontSettingCollection.Text);

                // Salva la cartella di lavoro
                workbook.Save("FontSettingCollectionTextDemo.xlsx");
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

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


