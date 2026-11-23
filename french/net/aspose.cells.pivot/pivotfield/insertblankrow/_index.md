---
title: "PivotField.InsertBlankRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique s’il faut insérer une ligne vide après chaque élément. Seulement pour les champs de ligne"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/insertblankrow/
---
## PivotField.InsertBlankRow property

Indique s'il faut insérer une ligne vide après chaque élément. Uniquement pour les champs de ligne.

```csharp
public bool InsertBlankRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyInsertBlankRowDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B5"].Value = 5;
            sheet.Cells["A6"].Value = "Orange";
            sheet.Cells["B6"].Value = 8;
            
            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Définir la propriété InsertBlankRow
            PivotField rowField = pivotTable.RowFields[0];
            rowField.InsertBlankRow = true;
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldInsertBlankRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


