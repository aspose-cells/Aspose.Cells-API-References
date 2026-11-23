---
title: "Class DataSorterKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DataSorterKey classe. Représente la clé du trieur de données"
type: docs
url: /fr/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

Représente la clé du DataSorter.

```csharp
public class DataSorterKey
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | Obtient la couleur triée. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | Représente l'identifiant du type de jeu d'icônes. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | Représente le type de jeu d'icônes. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | Obtient l'index de la colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | Indique l'ordre du tri. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | Représente le type de tri. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // Créez un objet classeur et chargez un fichier modèle
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple à trier
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // Instanciez l'objet trieur de données
            DataSorter sorter = workbook.DataSorter;

            // Ajoutez une clé pour la première colonne (A) à trier par ordre croissant
            sorter.AddKey(0, SortOrder.Ascending);

            // Créez une zone de cellules (plage) à trier
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // Effectuez le tri
            sorter.Sort(worksheet.Cells, ca);

            // Enregistrez le fichier de sortie
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // Accéder à la DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // Itérez à travers les clés et affichez leurs propriétés
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


