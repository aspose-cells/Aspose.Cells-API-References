---
title: "PasteOptions.Transpose"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PasteOptions. True pour transposer les lignes et les colonnes lorsque la plage est collée. La valeur par défaut est False"
type: docs
url: /fr/net/aspose.cells/pasteoptions/transpose/
---
## PasteOptions.Transpose property

Vrai pour transposer les lignes et les colonnes lorsque la plage est collée. La valeur par défaut est Faux.

```csharp
public bool Transpose { get; set; }
```

### Exemples

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

            // Créer le style source et l'appliquer à la plage horizontale
            Style style = workbook.CreateStyle();
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
            sourceRange.SetStyle(style);

            // Créer des options de collage avec transposition
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.Formats;
            pasteOptions.Transpose = true;

            // Copier avec transposition vers une plage verticale
            Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
            targetRange.Copy(sourceRange, pasteOptions);

            // Enregistrez le classeur
            workbook.Save("TransposeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


