---
title: "HyperlinkCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HyperlinkCollection. Obtient l'élément Hyperlink à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/hyperlinkcollection/item/
---
## HyperlinkCollection indexer

Obtient l'élément [`Hyperlink`](../../hyperlink/) à l'index spécifié.

```csharp
public Hyperlink this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un lien hypertexte à la cellule A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.example.com");
            
            // Accédez au premier lien hypertexte en utilisant la propriété Item et définissez le texte d'affichage
            worksheet.Hyperlinks[0].TextToDisplay = "Click Here";
            
            // Définir le style du lien hypertexte (texte bleu souligné)
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.Underline = FontUnderlineType.Single;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../../hyperlink/)
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


