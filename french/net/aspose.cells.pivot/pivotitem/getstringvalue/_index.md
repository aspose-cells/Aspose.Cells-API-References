---
title: "PivotItem.GetStringValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotItem. Obtient la valeur chaîne de l'élément pivot. Si la valeur est nulle, elle renverra"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/getstringvalue/
---
## PivotItem.GetStringValue method

Obtient la valeur chaîne de l'élément pivot. Si la valeur est nulle, elle renverra ""

```csharp
public string GetStringValue()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodGetStringValueDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accédez à la première feuille de calcul et au tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Obtenez le premier champ de ligne et ses éléments pivot
            PivotField rowField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = rowField.PivotItems;
            
            // Démontrez la méthode GetStringValue()
            string itemValue = pivotItems[1].GetStringValue();
            Console.WriteLine("PivotItem value: " + itemValue);
            
            // Enregistrer le classeur modifié
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


