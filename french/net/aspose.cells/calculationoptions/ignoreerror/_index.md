---
title: "CalculationOptions.IgnoreError"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationOptions. Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées. L'erreur peut être une fonction non prise en charge, des liens externes, etc. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Indique si les erreurs rencontrées lors du calcul des formules doivent être ignorées. L'erreur peut être une fonction non prise en charge, des liens externes, etc. La valeur par défaut est true.

```csharp
public bool IgnoreError { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une plage nommée qui n'existe pas pour démontrer la gestion des erreurs
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // Calculer avec IgnoreError = false (générera une erreur)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // Calculer avec IgnoreError = true (supprimera l'erreur)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### Voir aussi

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


