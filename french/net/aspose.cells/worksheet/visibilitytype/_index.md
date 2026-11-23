---
title: "Worksheet.VisibilityType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Indique l'état de visibilité de cette feuille"
type: docs
url: /fr/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Indique l'état de visibilité de cette feuille.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des feuilles de calcul
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Définir différents types de visibilité pour chaque feuille de calcul
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // Enregistrez le classeur
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // Rechargez le classeur pour vérifier les paramètres de visibilité
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Afficher les types de visibilité
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### Voir aussi

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


