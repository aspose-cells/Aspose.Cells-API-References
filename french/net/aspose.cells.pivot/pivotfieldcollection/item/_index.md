---
title: "PivotFieldCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotFieldCollection. Obtient l'objet PivotField à l'index spécifique"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfieldcollection/item/
---
## PivotFieldCollection indexer (1 of 2)

Obtient l'objet PivotField à l'index spécifique.

```csharp
public PivotField this[int index] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et obtenir la première feuille
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter des champs aux zones
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Accédez au premier champ de ligne en utilisant la propriété Item et définissez IsAutoSort
            pivotTable.RowFields[0].IsAutoSort = true;
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotFieldCollection indexer (2 of 2)

Obtient l'objet PivotField du nom spécifique.

```csharp
public PivotField this[string name] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "A";
            ws.Cells["B2"].Value = 10;
            ws.Cells["A3"].Value = "B";
            ws.Cells["B3"].Value = 20;
            ws.Cells["A4"].Value = "A";
            ws.Cells["B4"].Value = 30;
            ws.Cells["A5"].Value = "B";
            ws.Cells["B5"].Value = 40;

            // Créer un tableau croisé dynamique
            int index = ws.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pTable = ws.PivotTables[index];
            
            // Ajouter des champs au tableau croisé dynamique
            pTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Démontrer l'utilisation de la propriété Item
            pTable.DataFields["Sum of Value"].IsAutoSort = true;
            pTable.DataFields["Sum of Value"].IsAscendSort = false;
            
            // Actualiser et calculer le tableau croisé dynamique
            pTable.RefreshData();
            pTable.CalculateData();
            
            // Enregistrez le classeur
            wb.Save("PivotFieldCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


