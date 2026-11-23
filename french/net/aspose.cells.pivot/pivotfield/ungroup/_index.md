---
title: "PivotField.Ungroup"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Dégrouper le champ pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

Dégrouper le champ pivot.

```csharp
public void Ungroup()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder au premier tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Dégrouper le champ de la première colonne
            pivotTable.ColumnFields[0].Ungroup();
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


