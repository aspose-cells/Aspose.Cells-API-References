---
title: "DataSorterKey.IconId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorterKey. Représente l'ID du type de jeu d'icônes"
type: docs
url: /fr/net/aspose.cells/datasorterkey/iconid/
---
## DataSorterKey.IconId property

Représente l'identifiant du type de jeu d'icônes.

```csharp
public int IconId { get; }
```

### Remarques

Ne prend effet que lorsque [`Type`](../type/) est Icon.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterKeyPropertyIconIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple avec des valeurs pouvant utiliser des jeux d'icônes
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

            // Créer un trieur de données et ajouter une clé
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // Trier les données
            sorter.Sort(worksheet.Cells, area);

            try
            {
                // Afficher la propriété IconId à partir des clés du trieur
                foreach (DataSorterKey key in sorter.Keys)
                {
                    Console.WriteLine($"IconId: {key.IconId}");
                    Console.WriteLine($"IconSetType: {key.IconSetType}");
                }

                // Enregistrez le classeur
                workbook.Save("IconIdDemo.xlsx");
                Console.WriteLine("IconId demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


