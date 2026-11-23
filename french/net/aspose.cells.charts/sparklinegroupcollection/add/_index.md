---
title: "SparklineGroupCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SparklineGroupCollection. Ajoute un SparklineGroup avec un Sparkline à la collection"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Ajoute un [`SparklineGroup`](../../sparklinegroup/) avec un [`Sparkline`](../../sparkline/) à la collection.

```csharp
public int Add(SparklineType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | SparklineType | Spécifie le type du groupe Sparkline. |

### Valeur de retour

[`SparklineGroup`](../../sparklinegroup/) object index.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodAddWithSparklineTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour les sparklines
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // Obtenir la collection de groupes Sparkline
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // Appelez la méthode Add avec le paramètre SparklineType
                int index = sparklineGroups.Add(SparklineType.Line);

                // Configurer le groupe Sparkline
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Ajoute un [`SparklineGroup`](../../sparklinegroup/) avec quelques [`Sparkline`](../../sparkline/) à la collection.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | SparklineType | Spécifie le type du groupe Sparkline. |
| dataRange | String | Spécifie la plage de données du groupe Sparkline. |
| isVertical | Boolean | Spécifie s'il faut tracer les sparklines de la plage de données par ligne ou par colonne. |
| locationRange | CellArea | Spécifie où placer les sparklines. |

### Valeur de retour

[`SparklineGroup`](../../sparklinegroup/) object index.

### Remarques

Cette méthode créera également des sparklines. Si *isVertical* est vrai, le nombre de lignes dans dataRange et locationRange doit être identique. Si *isVertical* est faux, le nombre de colonnes dans dataRange et locationRange doit être identique.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionMethodAddWithSparklineTypeStringBooleanCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour les sparklines
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // Ajouter un groupe Sparkline avec les paramètres spécifiés
            sheet.SparklineGroups.Add(
                SparklineType.Line, 
                "A1:C1", 
                false, 
                CellArea.CreateCellArea("D1", "D1")
            );
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


