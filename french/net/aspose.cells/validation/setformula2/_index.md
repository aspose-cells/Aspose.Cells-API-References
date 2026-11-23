---
title: "Validation.SetFormula2"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode de validation. Définit la valeur ou l'expression associée à cette validation"
type: docs
url: /fr/net/aspose.cells/validation/setformula2/
---
## Validation.SetFormula2 method

Définit la valeur ou l'expression associée à cette validation.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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

    public class ValidationMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les valeurs de référence d'exemple
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["B1"].PutValue(200);

            // Créer une validation de données pour la cellule C1
            ValidationCollection validations = worksheet.Validations;
            Validation validation = validations[validations.Add()];
            validation.AddArea(CellArea.CreateCellArea(0, 0, 2, 2)); // Applies to cell C1

            // Configurer les paramètres de validation
            validation.Type = ValidationType.Custom;
            validation.Operator = OperatorType.Between;
            validation.ShowError = true;
            validation.ErrorTitle = "Range Error";
            validation.ErrorMessage = "Value must be between A1 (100) and B1 (200)";

            try
            {
                // Définir les formules de validation en utilisant les types de paramètres requis
                validation.SetFormula1("=A1", false, false);
                validation.SetFormula2("=B1", false, false); // Demonstrate (String, Boolean, Boolean)

                Console.WriteLine("SetFormula2 executed successfully with formula '=B1'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("ValidationSetFormula2Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


