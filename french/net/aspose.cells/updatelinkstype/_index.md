---
title: "Énum UpdateLinksType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énum Aspose.Cells.UpdateLinksType. Représente la façon de mettre à jour les liens vers d'autres classeurs lorsque le classeur est ouvert"
type: docs
url: /fr/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

Représente la façon de mettre à jour les liens vers d'autres classeurs lorsque le classeur est ouvert.

```csharp
public enum UpdateLinksType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| UserSet | `0` | Inviter l'utilisateur à mettre à jour. |
| Never | `1` | Ne pas mettre à jour, et ne pas inviter l'utilisateur. |
| Always | `2` | Toujours mettre à jour. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir UpdateLinksType sur Toujours mettre à jour
            settings.UpdateLinksType = UpdateLinksType.Always;

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // Enregistrez le classeur
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // Afficher le paramètre actuel d'UpdateLinksType
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


