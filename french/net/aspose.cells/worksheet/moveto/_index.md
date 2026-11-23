---
title: "Worksheet.MoveTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Déplace la feuille vers un autre emplacement dans le classeur"
type: docs
url: /fr/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

Déplace la feuille vers un autre emplacement dans la feuille de calcul.

```csharp
public void MoveTo(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | Indice de la feuille de destination. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter plusieurs feuilles de calcul
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Ajouter une nouvelle feuille de calcul et la déplacer à la position 1
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


