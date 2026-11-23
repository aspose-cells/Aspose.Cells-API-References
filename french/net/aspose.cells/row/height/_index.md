---
title: "Row.Height"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient et définit la hauteur de la ligne en unités de points"
type: docs
url: /fr/net/aspose.cells/row/height/
---
## Row.Height property

Obtient et définit la hauteur de la ligne en unités de points.

```csharp
public double Height { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la hauteur de la ligne pour la première ligne
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // Ajouter des données à la ligne
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // Vérifier et afficher la hauteur de la ligne
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // Enregistrez le classeur
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


