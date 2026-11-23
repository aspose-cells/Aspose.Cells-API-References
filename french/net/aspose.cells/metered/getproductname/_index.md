---
title: "Metered.GetProductName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Metered. Obtient le nom du produit"
type: docs
url: /fr/net/aspose.cells/metered/getproductname/
---
## Metered.GetProductName method

Obtient le nom du produit

```csharp
public string GetProductName()
```

### Valeur de retour

nom du produit

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodGetProductNameDemo
    {
        public static void Run()
        {
            // Créer une instance metered
            Metered metered = new Metered();
            
            // Définir les clés metered (remplacez par les clés réelles)
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Obtenir et afficher le nom du produit
            string productName = metered.GetProductName();
            Console.WriteLine("Product Name: " + productName);

            // Démontrer l'utilisation de base avec une feuille de calcul simple
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("Product: " + productName);
            workbook.Save("MeteredProductDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


