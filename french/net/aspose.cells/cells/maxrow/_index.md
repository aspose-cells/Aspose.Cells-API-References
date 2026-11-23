---
title: "Cells.MaxRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Cells. Index maximal de ligne de la cellule contenant des données ou un style"
type: docs
url: /fr/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Indice de ligne maximal de la cellule contenant des données ou un style.

```csharp
public int MaxRow { get; }
```

### Remarques

Retourne -1 s'il n'existe aucune cellule contenant des données ou un style dans la feuille de calcul. Cette propriété doit parcourir et vérifier les cellules et les lignes dynamiquement, ce qui consomme du temps et ne doit pas être invoquée de façon répétée, par exemple en l'utilisant directement comme condition dans une boucle.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // Obtenir l'index maximal de ligne (à base zéro)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // Ajouter de nouvelles données dans la ligne suivante après la ligne maximale
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // Vérifier la nouvelle ligne maximale
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // Enregistrez le classeur
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


