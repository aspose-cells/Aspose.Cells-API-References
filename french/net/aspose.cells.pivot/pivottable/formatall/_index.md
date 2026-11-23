---
title: "PivotTable.FormatAll"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Formater toutes les cellules dans la zone du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/formatall/
---
## PivotTable.FormatAll method

Formate toutes les cellules dans la zone du tableau croisé dynamique

```csharp
public void FormatAll(Style style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | Style à formater |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatAllWithStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            
            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Créer et configurer le style
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            
            // Appliquer le style à l’ensemble du tableau croisé dynamique
            pivotTable.FormatAll(style);
            
            // Enregistrez le classeur
            workbook.Save("PivotTableFormatAllDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


