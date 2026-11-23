---
title: "DataSorter.SortLeftToRight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. True signifie que l'orientation du tri est de gauche à droite. False signifie que l'orientation du tri est de haut en bas. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

Vrai signifie que l'orientation du tri est de gauche à droite. Faux signifie que l'orientation du tri est de haut en bas. La valeur par défaut est faux.

```csharp
public bool SortLeftToRight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple (les colonnes seront traitées comme des lignes lorsque SortLeftToRight=true)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // Créer un trieur de données et le configurer pour trier de gauche à droite
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // Définir la clé de tri (l'indice de colonne devient indice de ligne lors du tri de gauche à droite)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // Définir la zone de tri (les lignes deviennent des colonnes lors du tri de gauche à droite)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // Effectuez le tri
            sorter.Sort(worksheet.Cells, area);

            // Enregistrer le résultat
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### Voir aussi

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


