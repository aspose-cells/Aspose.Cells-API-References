---
title: "PivotConditionalFormat.ApplyTo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotConditionalFormat. Applique le format conditionnel à la plage qui doit se trouver dans la région de données"
type: docs
url: /fr/net/aspose.cells.pivot/pivotconditionalformat/applyto/
---
## PivotConditionalFormat.ApplyTo method

Applique le format conditionnel à la plage qui doit se trouver dans la région de données.

```csharp
public void ApplyTo(int row, int column, PivotConditionFormatScopeType scope)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | La ligne sélectionnée. |
| column | Int32 | La colonne sélectionnée. |
| portée | PivotConditionFormatScopeType | La portée |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodApplyToWithInt32Int32PivotConditionFormatDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotTableIndex = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotTableIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Ajouter un format conditionnel
            PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
            PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
            
            // Démontrer la méthode ApplyTo avec des paramètres spécifiques
            pcf.ApplyTo(0, 1, PivotConditionFormatScopeType.Field);
            
            // Ajoutez une condition de format
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = System.Drawing.Color.LightGreen;
            
            // Calculez les données et enregistrez
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatApplyToDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


