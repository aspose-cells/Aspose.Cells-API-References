---
title: "Metered.GetConsumptionQuantity"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Metered. Obtient la taille du fichier de consommation"
type: docs
url: /fr/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Obtient la taille du fichier de consommation

```csharp
public static decimal GetConsumptionQuantity()
```

### Valeur de retour

quantité de consommation

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // Créer une instance metered
            Metered metered = new Metered();

            try
            {
                // Définir les clés mesurées (remplacer par les clés réelles en utilisation réelle)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // Obtenir la quantité de consommation
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // Afficher le résultat
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // Créer un classeur pour démontrer l'utilisation mesurée
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Ajouter des données pour montrer que le classeur fonctionne
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // Enregistrez le classeur
                workbook.Save("MeteredConsumptionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in metered operation: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


