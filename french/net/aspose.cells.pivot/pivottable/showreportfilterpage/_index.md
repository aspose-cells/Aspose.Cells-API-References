---
title: "PivotTable.ShowReportFilterPage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Affiche toutes les pages de filtre de rapport selon le champ de pivot ; le champ de pivot doit être situé dans les champs de page"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showreportfilterpage/
---
## PivotTable.ShowReportFilterPage method

Affiche toutes les pages de filtre de rapport selon le champ PivotField, le champ PivotField doit être situé dans les champs de page.

```csharp
public void ShowReportFilterPage(PivotField pageField)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| pageField | PivotField | L'objet PivotField |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageWithPivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("source.xlsx");
            
            // Accéder à la première feuille de calcul et au tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Afficher les pages de filtre de rapport pour chaque champ de page
            foreach (PivotField pageField in pivotTable.PageFields)
            {
                pivotTable.ShowReportFilterPage(pageField);
            }
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


