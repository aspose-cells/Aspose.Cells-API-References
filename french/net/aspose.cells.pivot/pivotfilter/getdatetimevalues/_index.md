---
title: "PivotFilter.GetDateTimeValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotFilter. Obtient les valeurs du filtre numérique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfilter/getdatetimevalues/
---
## PivotFilter.GetDateTimeValues method

Obtient les valeurs du filtre numérique.

```csharp
public DateTime[] GetDateTimeValues()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterMethodGetDateTimeValuesDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Date";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = DateTime.Now;
            cells["B2"].Value = 1000;
            cells["A3"].Value = DateTime.Now.AddDays(1);
            cells["B3"].Value = 2000;
            cells["A4"].Value = DateTime.Now.AddDays(2);
            cells["B4"].Value = 3000;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Ajouter un champ de ligne et appliquer un filtre de date
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.BaseFields[0].FilterByDate(PivotFilterType.DateBetween, DateTime.Now, DateTime.Now.AddDays(1));
            
            // Obtenir le filtre et démontrer GetDateTimeValues
            PivotFilter filter = pivotTable.BaseFields[0].GetFilters()[0];
            DateTime[] dateValues = filter.GetDateTimeValues();
            
            Console.WriteLine("Filter Type: " + filter.FilterType);
            Console.WriteLine("First Date Value: " + dateValues[0]);
            Console.WriteLine("Second Date Value: " + dateValues[1]);
        }
    }
}
```

### Voir aussi

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


