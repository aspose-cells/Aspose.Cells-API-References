---
title: "WebExtensionProperty.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionProperty. Obtient et définit un nom de propriété personnalisé"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionproperty/name/
---
## WebExtensionProperty.Name property

Obtient et définit le nom d’une propriété personnalisée.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Définir et démontrer la propriété Name
                property.Name = "SampleName";
                Console.WriteLine($"Initial Name: {property.Name}");

                // Modifier et afficher le nom mis à jour
                property.Name = "UpdatedName";
                Console.WriteLine($"Modified Name: {property.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [WebExtensionProperty](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


