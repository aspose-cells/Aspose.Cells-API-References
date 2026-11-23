---
title: "CellWatch.CellName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellWatch. Obtient et définit le nom de la cellule"
type: docs
url: /fr/net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Obtient et définit le nom de la cellule.

```csharp
public string CellName { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyCellNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des surveillances de cellules
            worksheet.CellWatches.Add("B5");
            worksheet.CellWatches.Add("C10");
            
            // Afficher les noms de cellules de toutes les surveillances
            Console.WriteLine("Cell Watches:");
            foreach (CellWatch watch in worksheet.CellWatches)
            {
                Console.WriteLine(watch.CellName);
            }
            
            // Ajouter une nouvelle surveillance et afficher son nom
            worksheet.CellWatches.Add("A1");
            Console.WriteLine("Added new watch: " + 
                worksheet.CellWatches[worksheet.CellWatches.Count - 1].CellName);
            
            // Enregistrez le classeur
            workbook.Save("CellWatchDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


