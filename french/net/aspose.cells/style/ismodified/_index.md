---
title: "Style.IsModified"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Style. Vérifie si les propriétés spécifiées du style ont été modifiées. Utilisé pour le style des ConditionalFormattings afin de vérifier si les propriétés spécifiées de ce style doivent être utilisées lors de l'application des ConditionalFormattings sur une cellule"
type: docs
url: /fr/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

Vérifie si les propriétés spécifiées du style ont été modifiées. Utilisé pour le style de ConditionalFormattings afin de vérifier si les propriétés spécifiées de ce style doivent être utilisées lors de l'application de ConditionalFormattings sur une cellule.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Drapeaux de modification du style |

### Valeur de retour

vrai si les propriétés spécifiées ont été modifiées

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenir le style de la cellule A1
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // Modifier le motif (arrière-plan) du style
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // Vérifier si le motif a été modifié
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // Afficher le résultat
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### Voir aussi

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


