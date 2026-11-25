---
title: "FontSettingCollection.AppendText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection. Aggiunge il testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

Aggiunge il testo.

```csharp
public void AppendText(string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodAppendTextWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Imposta il testo iniziale
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // Chiama il metodo AppendText per aggiungere testo aggiuntivo
                fontSettingCollection.AppendText("World!");

                // Visualizza il testo modificato
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // Salva la cartella di lavoro
                workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AppendText method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


