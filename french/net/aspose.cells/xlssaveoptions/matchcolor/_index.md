---
title: "XlsSaveOptions.MatchColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XlsSaveOptions. Indique si la couleur de police doit correspondre, car il y a 56 couleurs dans la palette de couleurs standard"
type: docs
url: /fr/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Indique si la couleur de police correspond, car il y a 56 couleurs dans la palette de couleurs standard.

```csharp
public bool MatchColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // Créer un classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la cellule B2 et définir du texte avec une couleur de police spécifique
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // Définir la couleur de la police en bleu
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // Créer des options d'enregistrement avec MatchColor défini sur true
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // Enregistrer le classeur avec les options
            workbook.Save("output.xls", saveOptions);

            // Recharger le fichier enregistré pour vérifier que la couleur a été conservée
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // Vérifier que la couleur de la police est toujours bleue
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### Voir aussi

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


