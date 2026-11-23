---
title: "CellsHelper.SignificantDigitsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsHelper. Obtient et définit le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. La valeur par défaut est G17"
type: docs
url: /fr/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Obtient et définit le type par défaut de chiffres significatifs pour la sortie des valeurs numériques. La valeur par défaut est G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Afficher la valeur actuelle de SignificantDigitsType
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Définir une nouvelle valeur de SignificantDigitsType
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Créer un classeur pour démontrer l'effet
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter une valeur numérique qui sera affectée par les chiffres significatifs
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Calculer les formules avec le type actuel de chiffres significatifs
                workbook.CalculateFormula();

                // Afficher le résultat
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Passer à un autre type de chiffres significatifs
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Recalculer avec le nouveau type de chiffres significatifs
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Enregistrez le classeur
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


