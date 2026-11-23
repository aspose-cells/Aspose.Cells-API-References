---
title: "Column.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Column. Obtient et définit la largeur de la colonne en nombre de caractères"
type: docs
url: /fr/net/aspose.cells/column/width/
---
## Column.Width property

Obtient et définit la largeur de la colonne en unités de caractères.

```csharp
public double Width { get; set; }
```

### Remarques

Pour les feuilles de calcul, la largeur de colonne est mesurée en nombre de caractères correspondant à la largeur maximale d'un chiffre des nombres 0~9 tels qu'ils sont rendus avec la police du style normal.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la largeur pour la colonne 3 (index 2)
            worksheet.Cells.Columns[2].Width = 25.5;
            
            // Définir la largeur pour la colonne 4 (index 3)
            worksheet.Cells.Columns[3].Width = 40.0;
            
            // Obtenir et afficher les largeurs
            Console.WriteLine("Column 3 Width: " + worksheet.Cells.Columns[2].Width);
            Console.WriteLine("Column 4 Width: " + worksheet.Cells.Columns[3].Width);
            
            // Enregistrez le classeur
            workbook.Save("ColumnWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


