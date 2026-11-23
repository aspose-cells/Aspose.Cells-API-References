---
title: "Validation.SetFormula1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode de validation. Définit la valeur ou l'expression associée à cette validation"
type: docs
url: /fr/net/aspose.cells/validation/setformula1/
---
## Validation.SetFormula1 method

Définit la valeur ou l'expression associée à cette validation.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La valeur ou l'expression associée à cette condition de format. |
| isR1C1 | Boolean | Indique si la formule est une formule R1C1. |
| isLocal | Boolean | Si la formule est formatée selon la locale. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodSetFormula1WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Préparer des données d'exemple dans la cellule B1
            worksheet.Cells["B1"].PutValue(100);

            // Créer une validation de données pour la cellule A1
            int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.Decimal;
            validation.Operator = OperatorType.GreaterOrEqual;
            validation.ShowError = true;
            validation.ErrorTitle = "Validation Error";
            validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";

            try
            {
                // Définir la formule faisant référence à B1 en utilisant la notation A1 (non-R1C1, non local)
                validation.SetFormula1("=B1", false, false);
                Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
            }

            // Enregistrer le classeur avec la validation
            workbook.Save("ValidationSetFormula1Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


