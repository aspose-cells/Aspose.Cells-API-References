---
title: "Classe Metered"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Metered. Fournit des méthodes pour définir la clé mesurée"
type: docs
url: /fr/net/aspose.cells/metered/
---
## Metered class

Fournit des méthodes pour définir la clé mesurée.

```csharp
public class Metered
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Metered](metered/)() | Initialise une nouvelle instance de cette classe. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetProductName](../../aspose.cells/metered/getproductname/)() | Obtient le nom du produit |
| [SetMeteredKey](../../aspose.cells/metered/setmeteredkey/)(string, string) | Définit la clé publique et privée mesurée. Si vous achetez une licence à compte, au démarrage de l'application, cette API doit être appelée, normalement cela suffit. Cependant, si le téléchargement des données de consommation échoue constamment et dépasse 24 heures, la licence sera mise en statut d'évaluation ; pour éviter ce cas, vous devez vérifier régulièrement le statut de la licence, et s'il est en statut d'évaluation, appeler à nouveau cette API. |
| static [GetConsumptionCredit](../../aspose.cells/metered/getconsumptioncredit/)() | Obtient le crédit de consommation |
| static [GetConsumptionQuantity](../../aspose.cells/metered/getconsumptionquantity/)() | Obtient la taille du fichier de consommation |
| static [IsMeteredLicensed](../../aspose.cells/metered/ismeteredlicensed/)() | Vérifiez si Metered est licencié |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredDemo
    {
        public static void MeteredExample()
        {
            // Créez une instance de la classe Metered
            Metered metered = new Metered();

            // Définissez la clé mesurée
            string publicKey = "YourPublicKey";
            string privateKey = "YourPrivateKey";
            metered.SetMeteredKey(publicKey, privateKey);

            // Obtenez et affichez le nom du produit
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Code supplémentaire pour démontrer comment l'instance peut être utilisée
            // Par exemple, créer un classeur et l'enregistrer
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            workbook.Save("MeteredExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


