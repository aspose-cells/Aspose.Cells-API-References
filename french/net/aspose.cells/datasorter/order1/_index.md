---
title: "DataSorter.Order1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataSorter. Représente l'ordre de tri de la première clé"
type: docs
url: /fr/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

Représente l'ordre de tri de la première clé.

```csharp
public SortOrder Order1 { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // Définir les propriétés du trieur de données
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // Définir la plage de tri
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // Effectuez le tri
            sorter.Sort(worksheet.Cells, area);
            
            // Enregistrez le classeur
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


