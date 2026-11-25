---
title: "Shape.FormatCharacters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Formatta alcuni caratteri con le impostazioni del carattere"
type: docs
url: /it/net/aspose.cells.drawing/shape/formatcharacters/
---
## Shape.FormatCharacters method

Formatta alcuni caratteri con le impostazioni del carattere.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startIndex | Int32 | L'indice di partenza. |
| lunghezza | Int32 | La lunghezza. |
| font | Font | L'impostazione del font. |
| flag | StyleFlag | Il flag dell'impostazione del font. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi una casella di testo al foglio di lavoro
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text Formatting";
            
            // Crea un font con le proprietà desiderate
            Aspose.Cells.Font font = textBox.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            
            // Crea un flag di stile per specificare quali proprietà applicare
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            
            // Applica formattazione a caratteri specifici
            textBox.FormatCharacters(0, 6, font, flag);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [StyleFlag](../../../aspose.cells/styleflag/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


