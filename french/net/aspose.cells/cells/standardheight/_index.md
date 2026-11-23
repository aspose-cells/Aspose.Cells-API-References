---
title: "Cells.StandardHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points"
type: docs
url: /fr/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Obtient ou définit la hauteur de ligne par défaut dans cette feuille de calcul, en points.

```csharp
public double StandardHeight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenez et affichez la hauteur standard
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // Définissez une nouvelle hauteur standard
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // Enregistrez le classeur
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


