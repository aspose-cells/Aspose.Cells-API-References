---
title: "PivotTable.RefreshDataOnOpeningFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les données sont rafraîchies lors de l'ouverture du fichier"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/refreshdataonopeningfile/
---
## PivotTable.RefreshDataOnOpeningFile property

Indique s'il faut actualiser les données lors de l'ouverture du fichier.

```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDataOnOpeningFileDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Banana";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Orange";
            cells["B4"].Value = 3000;

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Définir la propriété RefreshDataOnOpeningFile
            pivotTable.RefreshDataOnOpeningFile = false;

            // Enregistrez le classeur
            workbook.Save("PivotTableRefreshDataOnOpeningFileDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


