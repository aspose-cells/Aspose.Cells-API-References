---
title: "AutoFilter.MatchBlanks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Correspond à toutes les cellules vides de la liste"
type: docs
url: /fr/net/aspose.cells/autofilter/matchblanks/
---
## AutoFilter.MatchBlanks method

Correspond à toutes les cellules vides de la liste.

```csharp
public void MatchBlanks(int fieldIndex)
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
    public class AutoFilterMethodMatchBlanksWithInt32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple avec quelques cellules vides
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Laisser C2 vide
            
            worksheet.Cells["A3"].PutValue("Data3");
            // Laisser B3 vide
            worksheet.Cells["C3"].PutValue("Data6");
            
            // Appliquer le filtre automatique
            worksheet.AutoFilter.Range = "A1:C3";
            AutoFilter filter = worksheet.AutoFilter;
            
            // Filtrer pour n'afficher que les lignes avec des cellules vides dans la colonne 3 (C)
            filter.MatchBlanks(2); // Column index is 0-based
            
            // Actualiser le filtre
            filter.Refresh();
            
            // Enregistrez le classeur
            workbook.Save("AutoFilterMatchBlanksDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


