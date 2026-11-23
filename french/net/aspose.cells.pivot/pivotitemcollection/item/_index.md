---
title: "PivotItemCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotItemCollection. Obtient l’objet PivotItem à l’index spécifié."
type: docs
url: /fr/net/aspose.cells.pivot/pivotitemcollection/item/
---
## PivotItemCollection indexer (1 of 2)

Obtient l’objet PivotItem à l’index spécifié.

```csharp
public PivotItem this[int index] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;
            
            // Créer un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Accédez aux éléments Pivot en utilisant la propriété Item
            PivotItemCollection pivotItems = pivotTable.RowFields[0].PivotItems;
            
            // Démontrer l'utilisation de la propriété Item
            Console.WriteLine("First pivot item: " + pivotItems[0].Name);
            Console.WriteLine("Second pivot item: " + pivotItems[1].Name);
            Console.WriteLine("Third pivot item: " + pivotItems[2].Name);
        }
    }
}
```

### Voir aussi

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotItemCollection indexer (2 of 2)

Obtient le [`PivotItem`](../../pivotitem/) par le nom spécifié.

```csharp
public PivotItem this[string itemValue] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Ajouter une nouvelle feuille de calcul pour le tableau croisé dynamique
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Ajouter un tableau croisé dynamique
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Configurer le tableau croisé dynamique
            pivotTable.RowFields["Vendor"].SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Actualiser et calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Démontre l’utilisation de la propriété Item et les opérations de déplacement
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Accédez aux éléments en utilisant la propriété Item
            items["4H12"].Move(0, true);
            items["DIF400"].Move(-1, true);
            
            pivotTable.CalculateData();
            
            items["CA32"].Move(0, true);
            items["AAA3"].Move(-1, true);

            // Enregistrez le classeur
            workbook.Save("PivotItemCollectionDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


