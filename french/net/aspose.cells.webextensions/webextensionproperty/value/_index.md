---
title: "WebExtensionProperty.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionProperty. Obtient et définit une valeur de propriété personnalisée"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionproperty/value/
---
## WebExtensionProperty.Value property

Obtient et définit la valeur d’une propriété personnalisée.

```csharp
public string Value { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));

                // Définir et démontrer la propriété Value
                property.Value = "SampleValue123";
                Console.WriteLine($"Initial Value: {property.Value}");

                // Modifier et afficher la valeur mise à jour
                property.Value = "UpdatedValue456";
                Console.WriteLine($"Modified Value: {property.Value}");
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


