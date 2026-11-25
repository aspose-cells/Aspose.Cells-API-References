---
title: "FontSettingCollection.InsertText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection. Inserisce l'indice nella posizione"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/inserttext/
---
## FontSettingCollection.InsertText method

Inserisce l'indice nella posizione.

```csharp
public void InsertText(int index, string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice di partenza. |
| testo | String | Il testo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            var fontSettingCollection = textBox.TextBody;

            // Imposta il testo iniziale
            fontSettingCollection.Text = "Initial Text";

            try
            {
                // Chiama il metodo InsertText per inserire il testo all'indice 7
                fontSettingCollection.InsertText(7, " Inserted");

                // Visualizza il testo modificato
                Console.WriteLine("Text after insertion: " + fontSettingCollection.Text);
                
                // Salva la cartella di lavoro
                workbook.Save("FontSettingCollectionInsertTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing InsertText method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


