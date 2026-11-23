---
title: "DataSorterKey.Color"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorterKey. Obtient la couleur triée"
type: docs
url: /fr/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

Obtient la couleur triée.

```csharp
public Color Color { get; }
```

### Remarques

Ne prend effet que lorsque [`Type`](../type/) est CellColor ou FontColor.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
    {
        public static void Run()
        {
            // Créer un objet classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Créer un trieur de données et ajouter une clé
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Trier les données
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // Afficher la propriété couleur à partir des clés
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### Voir aussi

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


