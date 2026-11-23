---
title: "PivotField.HideItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Définit si l'élément PivotItem spécifique dans un champ de données est masqué."
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Définit si l'élément PivotItem spécifique dans un champ de données est masqué.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(int index, bool isHidden)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | l'index du pivotItem dans le pivotField. |
| isHidden | Boolean | si le PivotItem spécifique est masqué |

### Remarques

NOTE: Cette méthode est maintenant obsolète. Au lieu de cela, veuillez utiliser la propriété PivotField.PivotItems[int].IsHidden à la place. Cette méthode sera supprimée 12 mois plus tard à compter d'août 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur avec un tableau croisé dynamique d'exemple
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Données d'exemple pour le tableau croisé dynamique
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("PO-23-05");
            sheet.Cells["A3"].PutValue("PO-23-06");
            sheet.Cells["A4"].PutValue("PO-23-05");
            sheet.Cells["A5"].PutValue("PO-23-07");
            
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(1500);
            sheet.Cells["B5"].PutValue(3000);

            // Créer un tableau croisé dynamique
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Masquer les éléments qui ne sont pas "PO-23-05"
            for (int i = 0; i < pivotField.ItemCount; i++)
            {
                pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
            }
            
            // Calculer le tableau croisé dynamique
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldHideItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Définit si l'élément PivotItem spécifique dans un champ de données est masqué.

```csharp
[Obsolete("Use PivotField.PivotItems[string].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(string itemValue, bool isHidden)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| itemValue | String | Le nom du pivotItem dans le pivotField. |
| isHidden | Boolean | Indique si le PivotItem spécifique est masqué |

### Remarques

NOTE: Cette méthode est maintenant obsolète. Au lieu de cela, veuillez utiliser la propriété PivotField.PivotItems[string].IsHidden à la place. Cette méthode sera supprimée 12 mois plus tard à compter d'août 2026. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodHideItemWithStringBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Appelez la méthode HideItem avec les paramètres (String, Boolean)
                pivotField.HideItem("Apple", true);

                Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
                Console.WriteLine("Apple items are now hidden in the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HideItem method: {ex.Message}");
            }

            // Enregistrer le résultat
            workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


