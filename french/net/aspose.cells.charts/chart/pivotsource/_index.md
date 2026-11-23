---
title: "Chart.PivotSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. La source est les données du tableau croisé dynamique. Si PivotSource n’est pas vide, le graphique est un PivotChart"
type: docs
url: /fr/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

La source est les données du tableau croisé dynamique. Si PivotSource n'est pas vide, le graphique est un PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Remarques

Si le tableau croisé dynamique "PivotTable1" se trouve dans la feuille de calcul "Sheet1" du fichier "Book1.xls". Le pivotSource pourrait être "[Book1.xls]Sheet1!PivotTable1" si le graphique et le tableau croisé dynamique ne sont pas dans le même classeur. Si vous définissez cette propriété, le paramètre de source de données précédent sera perdu.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPivotSourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;
            
            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source pivot pour le graphique
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Actualiser les données pivot et le graphique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // Enregistrez le classeur
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


