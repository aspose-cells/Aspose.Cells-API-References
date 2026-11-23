---
title: "Metered.GetConsumptionCredit"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Metered. Obtient le crédit de consommation"
type: docs
url: /fr/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

Obtient le crédit de consommation

```csharp
public static decimal GetConsumptionCredit()
```

### Valeur de retour

quantité de consommation

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // Créer une instance de la classe Metered
            Metered metered = new Metered();

            try
            {
                // Appeler la méthode GetConsumptionCredit de façon statique
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // Afficher le résultat
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // Créer un classeur simple pour démontrer l'effet (bien que GetConsumptionCredit ne modifie pas le classeur)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Ajouter les informations de crédit de consommation à la feuille de calcul
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // Enregistrez le classeur
                workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error getting consumption credit: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


