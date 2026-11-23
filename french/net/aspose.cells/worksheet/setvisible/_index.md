---
title: "Worksheet.SetVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Définit les options de visibilité"
type: docs
url: /fr/net/aspose.cells/worksheet/setvisible/
---
## Worksheet.SetVisible method

Définit les options visibles.

```csharp
public void SetVisible(bool isVisible, bool ignoreError)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isVisible | Boolean | Indique si la feuille de calcul est visible |
| ignoreError | Boolean | Indique s'il faut ignorer l'erreur si cette option n'est pas valide. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSetVisibleWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Définir la visibilité des feuilles de calcul
            // Premier paramètre : isVisible - false pour masquer la feuille
            // Deuxième paramètre : ignoreError - true pour ignorer l'erreur si la feuille ne peut pas être masquée
            workbook.Worksheets["Sheet2"].SetVisible(false, true);
            workbook.Worksheets["Sheet3"].SetVisible(false, true);

            // Enregistrez le classeur
            workbook.Save("WorksheetVisibilityDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


