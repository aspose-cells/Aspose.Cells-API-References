---
title: "Énumération CellValueFormatStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.CellValueFormatStrategy. Spécifie comment appliquer le style à la valeur de la cellule"
type: docs
url: /fr/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

Spécifie comment appliquer le style à la valeur de la cellule.

```csharp
public enum CellValueFormatStrategy
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Non formaté. |
| CellStyle | `1` | Uniquement formaté avec le style original de la cellule. |
| DisplayStyle | `2` | Formaté avec le style affiché de la cellule. |
| DisplayString | `3` | Obtient la chaîne affichée dans MS Excel. La principale différence avec DisplayStyle est que cette option prend également en compte l'effet de la largeur de colonne. Si la largeur de colonne est trop petite pour afficher la chaîne formatée complètement, "#" peut être affiché, comme le fait MS Excel. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // Appliquer différentes CellValueFormatStrategy pour démontrer leurs effets
            // Aucun : Non formaté
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle : Uniquement formaté avec le style original de la cellule
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle : Formaté avec le style affiché de la cellule
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString : Obtient la chaîne affichée dans MS Excel
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // Enregistrer le classeur dans un fichier
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


