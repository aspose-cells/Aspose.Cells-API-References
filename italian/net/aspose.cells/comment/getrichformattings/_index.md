---
title: "Comment.GetRichFormattings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Comment. Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri nel testo del commento"
type: docs
url: /it/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo del commento.

```csharp
public FontSetting[] GetRichFormattings()
```

### Valore di ritorno

Tutti gli oggetti Characters

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // Ottieni formattazioni di testo ricco
            FontSetting[] formattings = comment.GetRichFormattings();

            // Visualizza le informazioni di formattazione
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


