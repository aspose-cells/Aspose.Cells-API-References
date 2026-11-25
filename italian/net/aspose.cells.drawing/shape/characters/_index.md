---
title: "Shape.Characters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo"
type: docs
url: /it/net/aspose.cells.drawing/shape/characters/
---
## Shape.Characters method

Restituisce un oggetto Characters che rappresenta un intervallo di caratteri all'interno del testo.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice dell'inizio del carattere. |
| lunghezza | Int32 | Il numero di caratteri. |

### Valore di ritorno

Oggetto Characters.

### Osservazioni

Questo metodo funziona solo su forme con titolo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma con testo.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "Sample Text";

            // Ottieni i caratteri dall'indice 0 con lunghezza 4
            FontSetting fontSetting = shape.Characters(0, 4);
            
            // Modifica le impostazioni del font
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.Size = 14;
            fontSetting.Font.IsBold = true;

            // Salva la cartella di lavoro
            workbook.Save("ShapeCharactersDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


