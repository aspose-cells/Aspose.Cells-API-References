---
title: "Classe CustomImplementationFactory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CustomImplementationFactory. Fabrique permettant de créer certaines instances qui peuvent être réimplémentées par l'utilisateur à des fins spécifiques"
type: docs
url: /fr/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Fabrique pour créer certaines instances qui peuvent être réimplémentées par l'utilisateur à des fins spécifiques.

```csharp
public class CustomImplementationFactory
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Créez un CultureInfo à partir de l'ID fourni. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | Créez une instance de MemoryStream ou d'une implémentation personnalisée de MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | Créez une instance de MemoryStream ou d'une implémentation personnalisée de MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Créez une instance de générateur de nombres aléatoires. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;
    using System.IO;

    public class CustomImplementationFactoryDemo
    {
        public static void CustomImplementationFactoryExample()
        {
            // Créez une instance de CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Démontrez la méthode CreateMemoryStream sans paramètres
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Démontrez la méthode CreateMemoryStream avec le paramètre de capacité
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Démontrez la méthode CreateCultureInfo
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Démontrez la méthode CreateRandomInstance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Exemple d'utilisation de la fabrique avec CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


