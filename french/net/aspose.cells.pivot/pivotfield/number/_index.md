---
title: "PivotField.Number"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Représente le format d’affichage intégré des nombres et des dates"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Représente le format d'affichage intégré des nombres et des dates.

```csharp
public int Number { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNumberDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
            sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
            sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
            
            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Ajouter un champ de date à la zone des colonnes et définir le format numérique
            int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField field = pivot.ColumnFields[fieldIndex];
            field.Number = 16; // d-mmm format
            
            // Actualiser et calculer le tableau croisé dynamique
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldNumberDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


