---
title: "Enum HtmlCrossType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.HtmlCrossType. Représente cinq types de chaîne de croix html"
type: docs
url: /fr/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Représente cinq types de chaîne croisée HTML.

```csharp
public enum HtmlCrossType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Affichage similaire à MS Excel, dépend de la cellule suivante. Si la cellule suivante est nulle, la chaîne sera croisée, sinon elle sera tronquée |
| MSExport | `1` | Afficher la chaîne comme MS Excel lors de l'exportation html. |
| Cross | `2` | Afficher la chaîne de croix HTML, cette performance pour la création de gros fichiers html sera plus de dix fois plus rapide que de définir la valeur sur Default ou FitToCell. |
| CrossHideRight | `3` | Afficher la chaîne de croix HTML et masquer la chaîne de droite lorsque les textes se chevauchent. |
| FitToCell | `4` | Affichage uniquement de la chaîne à l'intérieur de la largeur de la cellule. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // Créer des options d'enregistrement HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Définir le type de croix sur MSExport
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // Enregistrer le classeur avec les options HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


