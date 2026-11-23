---
title: "AutoFilter.FilterTop10"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode AutoFilter. Filtre les 10 premiers éléments de la liste"
type: docs
url: /fr/net/aspose.cells/autofilter/filtertop10/
---
## AutoFilter.FilterTop10 method

Filtrer les 10 meilleurs éléments de la liste

```csharp
public void FilterTop10(int fieldIndex, bool isTop, bool isPercent, int itemCount)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | Le décalage entier du champ sur lequel vous souhaitez baser le filtre (à partir de la gauche de la liste ; le champ le plus à gauche est le champ 0). |
| isTop | Boolean | Indique si le filtre provient du haut ou du bas |
| isPercent | Boolean | Indique si les éléments sont en pourcentage ou en nombre |
| itemCount | Int32 | Le nombre d'éléments |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodFilterTop10WithInt32BooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple (5 lignes x 3 colonnes avec des valeurs numériques)
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Numbers");
            cells["A2"].PutValue(50);
            cells["A3"].PutValue(30);
            cells["A4"].PutValue(80);
            cells["A5"].PutValue(20);
            cells["A6"].PutValue(90);

            // Définir la plage du filtre automatique
            worksheet.AutoFilter.Range = "A1:A6";

            // Appliquer le filtre des 10 premiers (affichant les 2 premiers éléments)
            worksheet.AutoFilter.FilterTop10(0, true, false, 2);

            // Actualiser le filtre
            worksheet.AutoFilter.Refresh();

            // Enregistrez le classeur
            workbook.Save("FilterTop10Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


