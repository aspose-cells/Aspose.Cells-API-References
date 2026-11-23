---
title: "Worksheet.IsRulerVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique si la règle est visible. Cette propriété n'est appliquée que pour l'aperçu des sauts de page"
type: docs
url: /fr/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Indique si la règle est visible. Cette propriété n'est appliquée que pour l'aperçu des sauts de page.

```csharp
public bool IsRulerVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir la feuille de calcul en vue Mise en page où la règle est visible
            worksheet.ViewType = ViewType.PageLayoutView;

            // Basculer la visibilité de la règle
            worksheet.IsRulerVisible = true;

            // Afficher l'état actuel de visibilité de la règle
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // Enregistrez le classeur
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


