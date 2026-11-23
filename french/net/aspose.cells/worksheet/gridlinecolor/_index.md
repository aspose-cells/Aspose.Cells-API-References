---
title: "Worksheet.GridlineColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Worksheet property. Obtient et définit la couleur de la ligne de grille"
type: docs
url: /fr/net/aspose.cells/worksheet/gridlinecolor/
---
## Worksheet.GridlineColor property

Obtient et définit la couleur de la ligne de grille

```csharp
public Color GridlineColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la couleur de la ligne de grille sur rouge
            worksheet.GridlineColor = Color.Red;
            
            // Enregistrez le classeur
            string outputPath = "GridlineColorDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Gridline color set to red and saved to: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


