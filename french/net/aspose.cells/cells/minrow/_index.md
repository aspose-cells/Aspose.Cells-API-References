---
title: "Cells.MinRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Indice de ligne minimum de la cellule contenant des données ou un style"
type: docs
url: /fr/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Indice de ligne minimal de la cellule contenant des données ou un style.

```csharp
public int MinRow { get; }
```

### Remarques

Cette propriété doit itérer et vérifier les cellules et les lignes dynamiquement, il s’agit donc d’un processus gourmand en temps et ne doit pas être invoquée de façon répétée, par exemple en l’utilisant directement comme condition dans une boucle.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données pour démontrer MinRow
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // Afficher les informations de MinRow
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // Effacer le contenu à partir de MinRow
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // Vérifier l'effacement en contrôlant si les cellules sont vides
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


