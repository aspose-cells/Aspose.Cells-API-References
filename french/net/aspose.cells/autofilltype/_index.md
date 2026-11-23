---
title: "Enum AutoFillType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.AutoFillType enum. Représente le type de remplissage automatique"
type: docs
url: /fr/net/aspose.cells/autofilltype/
---
## AutoFillType enumeration

Représente le type de remplissage automatique.

```csharp
public enum AutoFillType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Copy | `1` | Copie la valeur et le format de la zone source vers la zone cible |
| Default | `0` | Remplit automatiquement la zone cible avec la valeur et le format. |
| Formats | `3` | Copie uniquement le format de la zone source vers la zone cible. |
| Series | `2` | Étend la valeur de la zone source vers la zone cible sous forme de série et copie le format vers la zone cible. |
| Values | `4` | Copie uniquement la valeur de la zone source vers la zone cible. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFillTypeDemo
    {
        public static void AutoFillTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez une plage (A1:A10) et remplissez-la avec quelques valeurs
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A10");
            for (int i = 0; i < 10; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            // Créez une plage cible (B1:B10)
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B10");

            //Erreur de type de série, un ticket a été créé
            // Utilisez la méthode AutoFill avec AutoFillType.Series pour remplir la plage cible
            //sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Utilisez la méthode AutoFill avec AutoFillType.Copy pour remplir la plage cible
            sourceRange.AutoFill(targetRange, AutoFillType.Copy);
            // Enregistrez le classeur
            workbook.Save("AutoFillTypeExample.xlsx");
            workbook.Save("AutoFillTypeExample.pdf");
        }
    }

}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


