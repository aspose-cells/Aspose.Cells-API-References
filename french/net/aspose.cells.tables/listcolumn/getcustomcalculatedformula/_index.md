---
title: "ListColumn.GetCustomCalculatedFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ListColumn. Obtient la formule de cette colonne de liste"
type: docs
url: /fr/net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

Obtient la formule de cette colonne de liste.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Indique si la formule doit être formatée en R1C1. |
| isLocal | Boolean | Indique si la formule doit être formatée selon la locale. |

### Valeur de retour

La formule de cette colonne de liste.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B1"].PutValue("Score");
            sheet.Cells["B2"].PutValue(85);
            sheet.Cells["B3"].PutValue(92);
            
            // Créer un objet de liste
            int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = sheet.ListObjects[index];
            
            // Ajouter une colonne calculée
            ListColumn calcColumn = listObject.ListColumns[1];
            calcColumn.Formula = "=WEEKNUM([@Score])";
            
            // Obtenir la formule calculée personnalisée
            string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
            
            // Afficher le résultat
            Console.WriteLine("Calculated Formula: " + formula);
        }
    }
}
```

### Voir aussi

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


