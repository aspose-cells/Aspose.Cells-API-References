---
title: "CellsHelper.SignificantDigits"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsHelper. Obtient et définit le nombre de chiffres significatifs. La valeur par défaut est 17"
type: docs
url: /fr/net/aspose.cells/cellshelper/significantdigits/
---
## CellsHelper.SignificantDigits property

Obtient et définit le nombre de chiffres significatifs. La valeur par défaut est 17.

```csharp
[Obsolete("Use SignificantDigitsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static int SignificantDigits { get; set; }
```

### Remarques

Il ne peut être que 15 ou 17 maintenant. NOTE : Ce membre est désormais obsolète. À la place, veuillez utiliser [`SignificantDigitsType`](../significantdigitstype/). Cette propriété sera supprimée 12 mois plus tard, à compter de juin 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertySignificantDigitsDemo
    {
        public static void Run()
        {
            // Définir les chiffres significatifs
            CellsHelper.SignificantDigits = 15;
            
            // Démontrez l'utilisation de la propriété
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            
            // Créez un classeur pour démontrer les chiffres significatifs dans les calculs
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez les valeurs qui seront affectées par les chiffres significatifs
            worksheet.Cells["A1"].PutValue(1.2345678912345678);
            worksheet.Cells["A2"].PutValue(1.2345678912345678);
            worksheet.Cells["A3"].Formula = "=A1+A2";
            
            // Calculez les formules avec les chiffres significatifs définis
            workbook.CalculateFormula();
            
            // Afficher les résultats
            Console.WriteLine("Value with significant digits: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


