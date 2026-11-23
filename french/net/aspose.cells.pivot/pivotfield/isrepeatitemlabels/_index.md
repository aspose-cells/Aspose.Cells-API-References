---
title: "PivotField.IsRepeatItemLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique s'il faut répéter les libellés du champ dans la région de ligne ou de colonne. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Indique s'il faut répéter les libellés du champ dans la région des lignes ou des colonnes. La valeur par défaut est fausse.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");

            // Accéder à la feuille de calcul contenant le tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // Accéder au tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];

            // Activer la répétition des libellés d'éléments pour le premier champ de ligne
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // Activer la répétition des libellés d'éléments pour le premier champ de colonne
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // Enregistrer le classeur modifié
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


