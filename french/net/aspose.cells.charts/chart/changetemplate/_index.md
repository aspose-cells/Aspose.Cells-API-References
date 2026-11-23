---
title: "Chart.ChangeTemplate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode du graphique. Change le type de graphique avec un modèle prédéfini"
type: docs
url: /fr/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

Modifiez le type de graphique avec un modèle prédéfini.

```csharp
public void ChangeTemplate(byte[] data)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| données | Byte[] | Les données du fichier de modèle de graphique (.crtx). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", false);

            // Obtenir les données du modèle à partir d'un autre fichier de graphique
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // Appeler la méthode ChangeTemplate avec un paramètre tableau d'octets
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // Afficher l'effet en enregistrant le classeur
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


