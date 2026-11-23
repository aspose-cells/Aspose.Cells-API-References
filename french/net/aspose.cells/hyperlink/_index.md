---
title: "Classe Hyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Hyperlink. Encapsule l'objet qui représente un hyperlien"
type: docs
url: /fr/net/aspose.cells/hyperlink/
---
## Hyperlink class

Encapsule l'objet qui représente un hyperlien.

```csharp
public class Hyperlink
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Représente l'adresse d'un hyperlien. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Obtient la plage de l'hyperlien. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Obtient le type de lien. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Renvoie ou définit le texte ScreenTip pour le lien hypertexte spécifié. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Représente le texte à afficher pour le lien hypertexte spécifié. La valeur par défaut est l'adresse du lien hypertexte. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Supprime ce lien hypertexte |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            
            // Ajout d'une nouvelle feuille de calcul à l'objet Workbook
            workbook.Worksheets.Add();
            
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajout d'un hyperlien vers une URL dans la cellule "A1"
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // Obtention d'un lien hypertexte par indice
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // Définition du texte d'affichage de ce lien hypertexte
            hyperlink.TextToDisplay = "Aspose";
            
            // Définition du texte ScreenTip pour le lien hypertexte
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // Enregistrement du fichier Excel
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


