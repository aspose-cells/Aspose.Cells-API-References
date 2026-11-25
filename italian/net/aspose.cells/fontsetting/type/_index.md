---
title: "FontSetting.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FontSetting. Ottiene il tipo di nodo di testo"
type: docs
url: /it/net/aspose.cells/fontsetting/type/
---
## FontSetting.Type property

Ottiene il tipo di nodo di testo.

```csharp
public virtual TextNodeType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;  // Added this using directive
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi testo a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Ottieni le impostazioni del carattere per i caratteri della cella
            FontSetting fontSetting = new FontSetting(0, 6, workbook.Worksheets);

            // Visualizza il valore corrente di Type
            Console.WriteLine("Current Type value: " + fontSetting.Type);

            // Dimostra come il Tipo influisce sull'elaborazione del testo
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                Console.WriteLine("The text is a standard text run.");
            }
            else if (fontSetting.Type == TextNodeType.TextParagraph)
            {
                Console.WriteLine("The text is part of a paragraph.");
            }
            else if (fontSetting.Type == TextNodeType.Equation)
            {
                Console.WriteLine("The text represents an equation.");
            }

            // Applica formattazione diversa in base al Tipo
            if (fontSetting.Type == TextNodeType.TextRun)
            {
                fontSetting.Font.Color = System.Drawing.Color.Red;
                fontSetting.SetWordArtStyle(PresetWordArtStyle.WordArtStyle1);
            }

            // Salva il risultato
            workbook.Save("FontSettingTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextNodeType](../../../aspose.cells.drawing.texts/textnodetype/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


