---
title: "Worksheet.PivotTables"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient tous les tableaux croisés dynamiques de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/pivottables/
---
## Worksheet.PivotTables property

Obtient tous les tableaux croisés dynamiques de cette feuille de calcul.

```csharp
public PivotTableCollection PivotTables { get; }
```

### Exemples

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPivotTablesDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de tableaux croisés dynamiques depuis la feuille de calcul
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Vérifier s'il existe des tableaux croisés dynamiques
            if (pivotTables.Count > 0)
            {
                // Obtenir le premier tableau croisé dynamique
                PivotTable pivotTable = pivotTables[0];
                
                // Effacer tous les filtres existants
                pivotTable.PivotFilters.Clear();
                
                // Actualiser les données du tableau croisé dynamique
                pivotTable.RefreshData();
                pivotTable.CalculateData();
                
                // Enregistrer le classeur modifié
                workbook.Save("PivotTableModified.xlsx");
            }
        }
    }
}
```

### Voir aussi

* class [PivotTableCollection](../../../aspose.cells.pivot/pivottablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


