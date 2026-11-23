---
title: "Cells.MinColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Indice de colonne minimal des cellules qui ont été instanciées dans la collection ne comprend pas la colonne où le style est défini pour toute la colonne mais aucune cellule n’a été instanciée dans celle‑ci."
type: docs
url: /fr/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Indice de colonne minimal des cellules qui ont été instanciées dans la collection (n'inclut pas la colonne où le style est défini pour toute la colonne mais aucune cellule n'a été instanciée).

```csharp
public int MinColumn { get; }
```

### Remarques

Cette propriété doit itérer et vérifier les cellules et les lignes dynamiquement, il s’agit donc d’un processus gourmand en temps et ne doit pas être invoquée de façon répétée, par exemple en l’utilisant directement comme condition dans une boucle.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de cellules
            Cells cells = worksheet.Cells;
            
            // Remplissez quelques données dans les colonnes 2, 3 et 4 (B, C, D)
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // Obtenez l’indice de colonne minimal qui contient des données
            int minColumn = cells.MinColumn;
            
            // Obtenez l’indice de colonne maximal qui contient des données
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // Effacez la colonne B pour démontrer le changement de MinColumn
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


