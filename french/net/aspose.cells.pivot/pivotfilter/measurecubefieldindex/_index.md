---
title: "PivotFilter.MeasureCubeFieldIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFilter. Spécifie l'index du champ du cube de mesure. Cette propriété n'est utilisée que par les filtres dans les pivots OLAP et indique sur quelle mesure un filtre de valeur doit s'appliquer"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/measurecubefieldindex/
---
## PivotFilter.MeasureCubeFieldIndex property

Spécifie l'index du champ cube de mesure. Cette propriété n'est utilisée que par les filtres dans les tableaux croisés dynamiques OLAP et indique sur quelle mesure un filtre de valeur doit s'appliquer.

```csharp
public int MeasureCubeFieldIndex { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureCubeFieldIndexDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et la remplir avec des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter des champs de ligne et de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Actualiser les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Ajoutez un filtre au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.BaseFields[0];
            
            // Créer et ajouter un filtre via PivotTable au lieu de PivotField
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            
            // Afficher MeasureCubeFieldIndex
            Console.WriteLine("MeasureCubeFieldIndex: " + filter.MeasureCubeFieldIndex);
            
            // Enregistrez le classeur
            workbook.Save("PivotFilterMeasureCubeFieldIndexDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


