---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomImplementationFactory. Créez une instance de générateur de nombres aléatoires"
type: docs
url: /fr/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Créez une instance de générateur de nombres aléatoires.

```csharp
public virtual Random CreateRandomInstance()
```

### Valeur de retour

instance de générateur de nombres aléatoires

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomImplementationFactoryMethodCreateRandomInstanceDemo
    {
        public static void Run()
        {
            try
            {
                // Créez une instance de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Appelez CreateRandomInstance pour obtenir un objet Random
                Random random = factory.CreateRandomInstance();

                // Démontrez la fonctionnalité de l'instance Random
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Montrez que la fabrique peut être utilisée avec CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateRandomInstance: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


