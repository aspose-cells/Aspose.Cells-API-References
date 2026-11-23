---
title: "Enum ViewType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ViewType enum. Représente le type d’affichage de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/viewtype/
---
## ViewType enumeration

Représente le type de vue de la feuille de calcul.

```csharp
public enum ViewType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| NormalView | `0` |  |
| PageBreakPreview | `1` |  |
| PageLayoutView | `2` |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ViewTypeDemo
    {
        public static void ViewTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez le type d’affichage de la feuille de calcul sur PageBreakPreview
            worksheet.ViewType = ViewType.PageBreakPreview;
            
            // Enregistrez le classeur
            workbook.Save("ViewTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


