---
title: "SeriesCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SeriesCollection. Ajoute la collection Series à un graphique"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

Ajoute la collection [`Series`](../../series/) à un graphique.

```csharp
public int Add(string dataArea, bool isVertical)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dataArea | String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | Boolean | Spécifie si la série doit être tracée à partir d’une plage de valeurs de cellules par ligne ou par colonne. Si vrai, [`Series`](../../series/) sera ajouté colonne par colonne |

### Valeur de retour

Renvoie le premier indice de l'ASeries ajouté dans le NSeries.

### Remarques

Si les données sont définies sur des cellules contiguës, utilisez deux-points pour les séparer. Par exemple, $C$2:$C$5. Si les données sont définies sur des cellules non contiguës, utilisez une virgule pour les séparer. Par exemple : ($C$2,$D$5). Cette méthode ne fait que traiter simplement *dataArea* comme plage de données. Si vous souhaitez vérifier intelligemment la méthode ChartCollection.Add().

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // Créer un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Ajouter des séries en utilisant des paramètres de chaîne et booléens
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // Enregistrez le classeur
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

Ajoute la collection [`Series`](../../series/) à un graphique.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| zone | String | Spécifie les valeurs à partir desquelles tracer la série de données |
| isVertical | Boolean | Spécifie s'il faut tracer la série à partir d'une plage de valeurs de cellules par ligne ou par colonne. |
| checkLabels | Boolean | Indique si la plage contient le nom de la série |

### Valeur de retour

Renvoie le premier indice de l'ASeries ajouté dans le NSeries.

### Remarques

Si les données sont définies sur des cellules contiguës, utilisez deux-points pour les séparer. Par exemple, $C$2:$C$5. Si les données sont définies sur des cellules non contiguës, utilisez une virgule pour les séparer. Par exemple, ($C$2,$D$5).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // Créer un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Ajouter des séries en utilisant la méthode Add avec des paramètres de chaîne et booléens
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // Enregistrez le classeur
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


