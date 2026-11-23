---
title: "PivotField.ShowInOutlineForm"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient ou définit une valeur indiquant si ce champ de ligne utilise la disposition en plan. S'applique uniquement aux champs de ligne"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/showinoutlineform/
---
## PivotField.ShowInOutlineForm property

Obtient ou définit une valeur indiquant si ce champ de ligne utilise la disposition en plan. S'applique uniquement aux champs de ligne.

```csharp
public bool ShowInOutlineForm { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowInOutlineFormDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Apple";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 25;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter un champ de ligne et démontrer ShowInOutlineForm
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Définir ShowInOutlineForm sur false
            rowField.ShowInOutlineForm = false;
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldShowInOutlineFormDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


