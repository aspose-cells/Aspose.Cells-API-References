---
title: "Énum VisibilityType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énum Aspose.Cells.VisibilityType. Représente les états de visibilité de la feuille"
type: docs
url: /fr/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

Représente les états de visibilité de la feuille.

```csharp
public enum VisibilityType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Visible | `0` | Indique que la feuille est visible. |
| Hidden | `1` | Indique que la feuille est masquée, mais peut être affichée par l'utilisateur via l'interface utilisateur. |
| VeryHidden | `2` | Indique que la feuille est masquée et ne peut pas être affichée dans l'interface utilisateur (UI). Cet état n'est disponible que par programmation. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le nom de la feuille de calcul
            worksheet.Name = "DemoSheet";

            // Définir la visibilité de la feuille de calcul sur Masqué
            worksheet.VisibilityType = VisibilityType.Hidden;

            // Enregistrez le classeur
            workbook.Save("VisibilityTypeExample.xlsx");

            // Sortie pour indiquer que le processus est terminé
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


