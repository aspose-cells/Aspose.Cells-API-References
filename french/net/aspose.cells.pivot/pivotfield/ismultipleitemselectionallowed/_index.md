---
title: "PivotField.IsMultipleItemSelectionAllowed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/ismultipleitemselectionallowed/
---
## PivotField.IsMultipleItemSelectionAllowed property

Indique si plusieurs éléments peuvent être sélectionnés dans le champ de page. La valeur par défaut est fausse.

```csharp
public bool IsMultipleItemSelectionAllowed { get; set; }
```

### Remarques

Uniquement pour les champs de page (filtre).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsMultipleItemSelectionAllowedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter des champs
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Accédez au champ de page et définissez la sélection multiple
            PivotField pageField = pivotTable.PageFields[0];
            pageField.IsMultipleItemSelectionAllowed = true;
            
            // Vérifier que la propriété a été définie
            Console.WriteLine("IsMultipleItemSelectionAllowed: " + pageField.IsMultipleItemSelectionAllowed);
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldIsMultipleItemSelectionAllowedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


