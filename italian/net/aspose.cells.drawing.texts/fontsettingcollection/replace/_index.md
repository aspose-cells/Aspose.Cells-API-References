---
title: "FontSettingCollection.Replace"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FontSettingCollection. Sostituisci il testo"
type: docs
url: /it/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

Sostituisce il testo.

```csharp
public void Replace(int index, int count, string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice di partenza. |
| conteggio | Int32 | Il conteggio dei caratteri. |
| testo | String | Il testo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // Chiama il metodo Replace per sostituire 8 caratteri a partire dall'indice 9 con il nuovo testo
                fontSettingCollection.Replace(9, 8, "replaced");

                // Visualizza il testo modificato
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // Salva la cartella di lavoro
                workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

Sostituisce il testo.

```csharp
public void Replace(string oldValue, string newValue)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| oldValue | String | Il testo vecchio. |
| nuovoValore | String | Il testo nuovo. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una forma e imposta il testo
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // Sostituisci il testo nella forma
            shape.TextBody.Replace("３４", "ABC");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


