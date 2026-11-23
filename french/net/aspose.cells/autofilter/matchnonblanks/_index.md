---
title: "AutoFilter.MatchNonBlanks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Correspond à toutes les cellules non vides de la liste"
type: docs
url: /fr/net/aspose.cells/autofilter/matchnonblanks/
---
## AutoFilter.MatchNonBlanks method

Correspond à toutes les cellules non vides de la liste.

```csharp
public void MatchNonBlanks(int fieldIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodMatchNonBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple avec quelques cellules vides
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(""); // Blank cell
            worksheet.Cells["B3"].PutValue(5);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(8);
            worksheet.Cells["A5"].PutValue(""); // Blank cell
            worksheet.Cells["B5"].PutValue(12);

            // Appliquer le filtre automatique pour n'afficher que les cellules non vides dans la colonne A (index 0)
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.MatchNonBlanks(0);
            worksheet.AutoFilter.Refresh();

            // Enregistrez le classeur
            workbook.Save("FilterNonBlanks.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


