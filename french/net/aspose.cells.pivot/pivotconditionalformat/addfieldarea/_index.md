---
title: "PivotConditionalFormat.AddFieldArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotConditionalFormat. Ajoute une zone de champ de tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotconditionalformat/addfieldarea/
---
## AddFieldArea(PivotFieldType, string) {#addfieldarea_1}

Ajoute une zone du champ du tableau croisé dynamique.

```csharp
public void AddFieldArea(PivotFieldType axisType, string fieldName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | Le type de région. |
| fieldName | String | Le nom du champ pivot. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypeStringDemo
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

            // Créez un tableau croisé dynamique - corrigé en obtenant le tableau croisé dynamique depuis l'index
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Ajouter un format conditionnel
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;
            
            // Démontrez AddFieldArea avec les paramètres PivotFieldType et chaîne
            pcf.AddFieldArea(PivotFieldType.Data, "Value");
            pcf.AddFieldArea(PivotFieldType.Row, "Category");

            // Ajoutez une condition de format
            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = "20";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundArgbColor = Color.LightGreen.ToArgb();

            // Calculez les données et enregistrez
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotConditionalFormatDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldArea(PivotFieldType, PivotField) {#addfieldarea}

Ajoute une zone du champ du tableau croisé dynamique.

```csharp
public void AddFieldArea(PivotFieldType axisType, PivotField field)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | Le type de région. |
| champ | PivotField | Le champ pivot. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotConditionalFormatMethodAddFieldAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 100;
            cells["B3"].Value = 150;
            cells["B4"].Value = 200;

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A5", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Ajoutez des champs aux zones du tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // First field (Fruit) as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Second field (Quantity) as data

            // Ajouter un format conditionnel
            int formatIndex = pivotTable.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivotTable.ConditionalFormats[formatIndex];
            
            // Démontrez AddFieldArea avec les paramètres PivotFieldType et PivotField
            pfc.AddFieldArea(PivotFieldType.Row, pivotTable.RowFields[0]);
            
            // Ajoutez une condition de format
            int conditionIndex = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition condition = pfc.FormatConditions[conditionIndex];
            condition.Formula1 = "100";
            condition.Operator = OperatorType.GreaterOrEqual;
            condition.Style.BackgroundColor = System.Drawing.Color.Red;

            // Enregistrez le classeur
            workbook.Save("PivotConditionalFormatExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


