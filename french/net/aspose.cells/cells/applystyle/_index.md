---
title: "Cells.ApplyStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cells. Applique des formats à l’ensemble d’une feuille de calcul"
type: docs
url: /fr/net/aspose.cells/cells/applystyle/
---
## Cells.ApplyStyle method

Applique des formats à une feuille de calcul entière.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | L'objet style qui sera appliqué. |
| flag | StyleFlag | Indicateurs qui spécifient les propriétés de formatage appliquées. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = wb.Worksheets[0];
            
            // Créez un style et définissez le retour à la ligne du texte
            Style style = wb.CreateStyle();
            style.IsTextWrapped = true;
            
            // Créez un indicateur de style et activez l’indicateur de retour à la ligne du texte
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Appliquez le style à toutes les cellules de la feuille de calcul
            sheet.Cells.ApplyStyle(style, flag);
            
            // Enregistrez le classeur
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


