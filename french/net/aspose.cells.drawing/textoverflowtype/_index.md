---
title: "Enum TextOverflowType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.TextOverflowType. Représente la façon dont le texte déborde verticalement ou horizontalement."
type: docs
url: /fr/net/aspose.cells.drawing/textoverflowtype/
---
## TextOverflowType enumeration

Représente la façon dont le texte déborde verticalement ou horizontalement.

```csharp
public enum TextOverflowType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Clip | `0` | Faites attention aux barrières supérieures et inférieures. Ne fournissez aucune indication qu'il y a du texte qui n'est pas visible. |
| Ellipsis | `1` | Faites attention aux barrières supérieures et inférieures. Utilisez des points de suspension pour indiquer qu'il y a du texte qui n'est pas visible. Seulement pour le débordement vertical. |
| Overflow | `2` | Faites déborder le texte sans tenir compte des barrières supérieures et inférieures. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassTextOverflowTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez une zone de texte au graphique
            TextBox textBox = chart.Shapes.AddTextBoxInChart(10, 10, 200, 50);

            // Définissez les propriétés de la zone de texte
            textBox.TextBody.TextAlignment.AutoSize = false;
            textBox.Text = "This is a long text that will demonstrate text overflow handling";
            
            // Définissez le type de débordement du texte
            textBox.TextVerticalOverflow = TextOverflowType.Clip;

            // Enregistrez le classeur
            workbook.Save("TextOverflowTypeDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


