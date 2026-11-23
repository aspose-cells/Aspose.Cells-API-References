---
title: "PivotItem.Index"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotItem. Obtient l'index de l'élément pivot dans le champ de cache"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

Obtient l'index de l'élément pivot dans le champ de cache.

```csharp
[Obsolete("Use PivotItem.Position property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Index { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotItem.Position . Cette méthode sera supprimée 6 mois plus tard à compter d'août 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIndexDemo
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
            
            // Ajouter le champ de ligne
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Ajouter le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Obtenez le champ de ligne
            PivotField rowField = pivotTable.RowFields[0];
            
            // Accédez aux éléments pivot en utilisant la propriété Index
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
                
                // Masquez le détail de l'élément en utilisant la propriété Index
                if (item.Value.ToString() == "Apple")
                {
                    rowField.HideItemDetail(item.Index, true);
                }
            }
            
            // Calculer et actualiser le tableau croisé dynamique
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Enregistrez le classeur
            workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


