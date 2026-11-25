---
title: "Shape.GetCharacters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo."
type: docs
url: /it/net/aspose.cells.drawing/shape/getcharacters/
---
## Shape.GetCharacters method

Restituisce tutti gli oggetti Characters che rappresentano un intervallo di caratteri all'interno del testo.

```csharp
[Obsolete("Use Shape.GetRichFormattings() instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetCharacters()
```

### Valore di ritorno

Tutti gli oggetti Characters

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Shape.GetRichFormattings(). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using System.Collections;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di casella di testo al foglio di lavoro con tutti i parametri richiesti
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            shape.Text = "Sample Text";

            // Ottieni i caratteri dalla forma
            ArrayList characters = shape.GetCharacters();

            // Visualizza le informazioni su ogni carattere
            foreach (FontSetting charSetting in characters)
            {
                Console.WriteLine($"Font: {charSetting.Font.Name}, Size: {charSetting.Font.Size}");
            }
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


