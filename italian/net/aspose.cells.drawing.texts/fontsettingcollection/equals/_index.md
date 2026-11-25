---
title: "FontSettingCollection.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection."
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/equals/
---
## FontSettingCollection.Equals method

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object |  |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una casella di testo al foglio di lavoro
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // Imposta del testo
            fontSettingCollection.Text = "Sample Text";

            try
            {
                // Crea un altro FontSettingCollection per il confronto
                var anotherTextBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var anotherFontSettingCollection = anotherTextBox.TextBody;
                anotherFontSettingCollection.Text = "Sample Text";

                // Chiama il metodo Equals per confrontare le due collezioni
                bool areEqual = fontSettingCollection.Equals(anotherFontSettingCollection);

                // Visualizza il risultato
                Console.WriteLine($"Are the FontSettingCollections equal? {areEqual}");

                // Salva la cartella di lavoro
                workbook.Save("FontSettingCollectionEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Equals: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


