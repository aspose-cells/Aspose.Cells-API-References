---
title: "PivotTable.AddCalculatedField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Ajoute un champ calculé au champ de tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

Ajoute un champ calculé au champ pivot.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom du champ calculé |
| formule | String | La formule du champ calculé. |
| dragToDataArea | Boolean | Vrai, faites glisser ce champ vers la zone de données immédiatement |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 150;
            cells["A4"].Value = "C";
            cells["B4"].Value = 200;

            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ajouter un champ calculé
            pivotTable.AddCalculatedField("DoubleSales", "=Sales*2", true);

            // Enregistrez le classeur
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

Ajoute un champ calculé au champ pivot et le fait glisser vers la zone de données.

```csharp
public void AddCalculatedField(string name, string formula)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom du champ calculé |
| formule | String | La formule du champ calculé. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(8);
            
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(3);
            worksheet.Cells["C4"].PutValue(10);

            // Créer une collection de tableaux croisés dynamiques
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Ajouter un tableau croisé dynamique et obtenir son indice
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            
            // Obtenir l'objet du tableau croisé dynamique
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Ajouter des champs à la zone de lignes
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Ajouter des champs de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Ajouter un champ calculé
            pivotTable.AddCalculatedField("Total", "=Price*Quantity");
            
            // Formater le champ de données
            pivotTable.DataFields["Total"].NumberFormat = "$#,##0.00";
            
            // Actualiser et calculer le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


