---
title: "TrendlineCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TrendlineCollection. Ajoute un objet Trendline à cette collection avec le type spécifié"
type: docs
url: /fr/net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Ajoute un objet [`Trendline`](../../trendline/) à cette collection avec le type spécifié.

```csharp
public int Add(TrendlineType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Type de Trendline. |

### Valeur de retour

[`Trendline`](../../trendline/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["B4"].PutValue(8);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter des données de série
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ajouter une courbe de tendance exponentielle à la première série
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            // Enregistrez le classeur
            workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Ajoute un objet [`Trendline`](../../trendline/) à cette collection avec le type et le nom spécifiés.

```csharp
public int Add(TrendlineType type, string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | TrendlineType | Type de Trendline. |
| name | String | Nom de la Trendline. |

### Valeur de retour

[`Trendline`](../../trendline/) object index.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Créer un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Ajouter une série et définir les données
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].Name = "Data Series";

            // Ajouter une Trendline avec TrendlineType et nom
            chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
            
            // Définir certaines propriétés de la Trendline
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            
            workbook.Save("TrendlineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


