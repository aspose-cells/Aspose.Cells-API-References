---
title: "PivotTable.ShowReportFilterPageByIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Afficher toutes les pages de filtre de rapport selon l'index de position dans les PageFields"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showreportfilterpagebyindex/
---
## PivotTable.ShowReportFilterPageByIndex method

Affiche toutes les pages de filtre de rapport selon l'index de position dans les champs de page.

```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| posIndex | Int32 | L'index de position dans les PageFields |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("PivotTable.xlsx");
            
            // Accéder à la première feuille de calcul contenant le tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Afficher les pages de filtre de rapport par index (position) du champ de page
            int pageFieldIndex = 0; // First page field
            pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
            
            // Enregistrez le classeur
            workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


