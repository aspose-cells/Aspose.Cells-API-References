---
title: "Range.CopyStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Copie les paramètres de style d'une plage source"
type: docs
url: /fr/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

Copie les paramètres de style depuis une plage source.

```csharp
public void CopyStyle(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| range | Range | Objet source [`Range`](../). |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // Ajoutez un style d'exemple à la plage source
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // Créer la feuille de calcul de destination
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // Créer la plage de destination et copier le style
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // Enregistrez le classeur
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


