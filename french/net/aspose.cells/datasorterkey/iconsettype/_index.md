---
title: "DataSorterKey.IconSetType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorterKey. Représente le type de jeu d'icônes"
type: docs
url: /fr/net/aspose.cells/datasorterkey/iconsettype/
---
## DataSorterKey.IconSetType property

Représente le type de jeu d'icônes.

```csharp
public IconSetType IconSetType { get; }
```

### Remarques

Ne prend effet que lorsque [`Type`](../type/) est Icon.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Créer un objet classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec un formatage conditionnel de jeu d'icônes
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Ajouter une mise en forme conditionnelle d'ensemble d'icônes
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = CellArea.CreateCellArea("A1", "A5");
            fcc.AddArea(area);
            fcc.AddCondition(FormatConditionType.IconSet);
            fcc[0].IconSet.Type = IconSetType.Arrows3;

            // Créer un trieur de données avec le type de jeu d'icônes
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Trier les données
            sorter.Sort(worksheet.Cells, area);

            // Afficher le type de jeu d'icônes à partir de la clé du trieur
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"IconSetType used for sorting: {key.IconSetType}");
            }

            // Enregistrez le classeur
            workbook.Save("IconSetTypeSortingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [IconSetType](../../iconsettype/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


