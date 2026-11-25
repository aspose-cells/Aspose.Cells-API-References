---
title: "PasteOptions.Transpose"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PasteOptions. True per trasporre righe e colonne quando l'intervallo viene incollato. Il valore predefinito è False"
type: docs
url: /it/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

True per trasporre righe e colonne quando l'intervallo è incollato. Il valore predefinito è False.

```csharp
public bool Transpose { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyTransposeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea lo stile di origine e applicalo all'intervallo orizzontale
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // Crea le opzioni di incolla con trasposizione
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // Copia con trasposizione in un intervallo verticale
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // Salva la cartella di lavoro
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


