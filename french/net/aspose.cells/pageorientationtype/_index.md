---
title: "Enum PageOrientationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.PageOrientationType. Représente les constantes d'orientation d'impression"
type: docs
url: /fr/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

Représente les constantes d'orientation d'impression.

```csharp
public enum PageOrientationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Landscape | `0` | Orientation paysage |
| Portrait | `1` | Orientation portrait |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez à la première feuille de calcul du classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à l'objet PageSetup de la feuille de calcul
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Définir l'orientation de la page sur Paysage
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // Enregistrer le classeur dans un fichier
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // Définir l'orientation de la page sur Portrait
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // Enregistrez le classeur dans un fichier différent
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


