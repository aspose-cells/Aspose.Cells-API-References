---
title: "StyleFlag.FontColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà StyleFlag. Verrà applicata l'impostazione del colore del carattere"
type: docs
url: /it/net/aspose.cells/styleflag/fontcolor/
---
## StyleFlag.FontColor property

L'impostazione del colore del carattere sarà applicata.

```csharp
public bool FontColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea uno stile personalizzato
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.BackgroundColor = System.Drawing.Color.LightGray;
            
            // Crea un flag di stile e abilita il colore del carattere e l'ombreggiatura della cella
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontColor = true;
            styleFlag.CellShading = true;
            
            // Applica lo stile alla cella A1 con i flag specificati
            worksheet.Cells["A1"].PutValue("Red Text on Gray Background");
            worksheet.Cells["A1"].SetStyle(style, styleFlag);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


