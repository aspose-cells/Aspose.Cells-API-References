---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomImplementationFactory. Créez un CultureInfo à partir de l'identifiant fourni"
type: docs
url: /fr/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Créez un CultureInfo à partir de l'ID fourni.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| lcid | Int32 |  |

### Valeur de retour

L'instance CultureInfo.

### Remarques

Cette implémentation est utile dans les situations suivantes : 1. Certaines cultures peuvent ne pas être prises en charge par l'environnement de l'utilisateur et la création du CultureInfo requis avec l'identifiant fourni peut entraîner une exception. Pour éviter l'exception, l'utilisateur peut remplacer cette méthode afin de fournir une instance CultureInfo valide pour la culture non prise en charge. 2. L'utilisateur peut souhaiter spécifier des propriétés personnalisées pour certaines cultures afin d'obtenir le résultat attendu lors du formatage. À cette fin, l'utilisateur peut remplacer cette méthode pour fournir l'instance CultureInfo avec les propriétés spécifiées par l'utilisateur. Veuillez noter que la propriété UseUserOverride de l'instance CultureInfo retournée peut influencer le résultat formaté. Si elle est false, certaines propriétés de l'instance CultureInfo retournée peuvent être remplacées par notre moteur de formatage intégré selon les exigences de formatage de différents scénarios. Si elle est true, nous ne modifierons aucune de ses propriétés et l'utiliserons directement pour formater les valeurs. Ainsi, si l'utilisateur a spécifié des propriétés personnalisées pour l'instance CultureInfo retournée, veuillez vous assurer que sa propriété UseUserOverride est true.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Créez une instance de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Appelez CreateCultureInfo avec un LCID valide (1033 pour l'anglais - États-Unis)
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Affichez les résultats
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // Démontrez la configuration de la fabrique dans CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


