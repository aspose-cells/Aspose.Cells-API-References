---
title: "FontSettingCollection.DeleteText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection. Elimina alcuni caratteri"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

Elimina alcuni caratteri.

```csharp
public void DeleteText(int index, int count)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice di partenza. |
| conteggio | Int32 | Il conteggio dei caratteri. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
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
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // Visualizza il testo originale
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // Chiama il metodo DeleteText per rimuovere 7 caratteri a partire dall'indice 5
                fontSettingCollection.DeleteText(5, 7);

                // Visualizza il testo modificato
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // Salva la cartella di lavoro
                workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


