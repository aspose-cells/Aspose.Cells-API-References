---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique s'il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

Indique s’il faut ajuster automatiquement la largeur des colonnes lors de la mise à jour

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la feuille de calcul contenant le tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // Accéder au tableau croisé dynamique
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Désactiver l'ajustement automatique de la largeur des colonnes lors de la mise à jour
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // Actualiser le tableau croisé dynamique pour appliquer les modifications
            worksheet.RefreshPivotTables();
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


