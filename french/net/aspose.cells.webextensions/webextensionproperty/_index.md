---
title: "Classe WebExtensionProperty"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionProperty. Représente une propriété personnalisée d’Office Add‑in"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionproperty/
---
## WebExtensionProperty class

Représente une propriété personnalisée d'Office Add-in.

```csharp
public class WebExtensionProperty
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Name](../../aspose.cells.webextensions/webextensionproperty/name/) { get; set; } | Obtient et définit le nom d’une propriété personnalisée. |
| [Value](../../aspose.cells.webextensions/webextensionproperty/value/) { get; set; } | Obtient et définit la valeur d’une propriété personnalisée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionsClassWebExtensionPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Créez une nouvelle instance de WebExtensionProperty
                WebExtensionProperty property = (WebExtensionProperty)Activator.CreateInstance(typeof(WebExtensionProperty));
                
                // Définissez les valeurs des propriétés
                property.Name = "SampleProperty";
                property.Value = "SampleValue";
                
                // Affiche les valeurs des propriétés
                Console.WriteLine($"Property Name: {property.Name}");
                Console.WriteLine($"Property Value: {property.Value}");
                
                Console.WriteLine("WebExtensionProperty demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in WebExtensionProperty demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


