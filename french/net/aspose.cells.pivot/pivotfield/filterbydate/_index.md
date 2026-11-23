---
title: "PivotField.FilterByDate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Filtre par valeurs de date du champ pivot de ligne ou de colonne"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/filterbydate/
---
## PivotField.FilterByDate method

Filtre par valeurs de date du champ pivot de ligne ou de colonne.

```csharp
public PivotFilter FilterByDate(PivotFilterType type, DateTime dateTime1, DateTime dateTime2)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | PivotFilterType | Le type de données de filtrage. |
| dateTime1 | DateTime | L'étiquette de date de la condition de filtre |
| dateTime2 | DateTime | L'étiquette de date supérieure de la condition de filtre entre |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterByDateWithPivotFilterTypeDateTimeDateTimDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple avec des dates
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2020, 9, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2020, 10, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2021, 9, 16));
            worksheet.Cells["A5"].PutValue(new DateTime(2021, 11, 5));

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:A5", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter le champ de date à la zone de colonne
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField pivotField = pivotTable.ColumnFields[fieldIndex];
            
            // Appliquer le filtre de date (dates de septembre entre 2020-2021)
            pivotField.FilterByDate(PivotFilterType.September, new DateTime(2020, 1, 1), new DateTime(2021, 12, 31));
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez les résultats
            workbook.Save("FilterByDateDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


