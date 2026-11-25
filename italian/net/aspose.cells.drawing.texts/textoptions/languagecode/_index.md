---
title: "TextOptions.LanguageCode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TextOptions. Ottiene e imposta la lingua dell'interfaccia utente"
type: docs
url: /it/net/aspose.cells.drawing.texts/textoptions/languagecode/
---
## TextOptions.LanguageCode property

Ottiene e imposta la lingua dell'interfaccia utente.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma e imposta il suo testo
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample text with language settings";

            // Imposta il codice lingua per le opzioni di testo della forma
            shape.TextOptions.LanguageCode = CountryCode.Japan;

            // Verifica e restituisci il codice lingua
            Console.WriteLine("Shape Text Language Code: " + shape.TextOptions.LanguageCode);

            // Salva la cartella di lavoro
            workbook.Save("TextOptionsLanguageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CountryCode](../../../aspose.cells/countrycode/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


