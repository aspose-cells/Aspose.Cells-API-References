---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotDateTimeRangeGroupSettings. Obtient l'élément interne du groupe"
type: docs
url: /fr/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Obtient l'interne du groupe.

```csharp
public double Interval { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul avec des données d'exemple
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Ajouter des données de date d'exemple
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // Ajouter une feuille de calcul de tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // Ajouter un tableau croisé dynamique
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Ajoutez le champ de date à la zone de lignes
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // Regrouper par jours avec un intervalle de 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // Étant donné que Interval est en lecture seule, nous devons le définir lors du regroupement
            // L'intervalle est en fait défini dans les paramètres de la méthode GroupBy
            // Ici nous vérifions simplement la valeur de l'intervalle
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // Enregistrez le classeur
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


