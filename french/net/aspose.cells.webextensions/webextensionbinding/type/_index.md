---
title: "WebExtensionBinding.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionBinding. Obtient et définit le type de liaison"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionbinding/type/
---
## WebExtensionBinding.Type property

Obtient et définit le type de liaison.

```csharp
public string Type { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle instance de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Définir la propriété Type
                binding.Type = "text";
                
                // Afficher la valeur actuelle de Type
                Console.WriteLine("Initial Type value: " + binding.Type);
                
                // Modifier la valeur de Type pour démontrer qu'elle est en lecture/écriture
                binding.Type = "range";
                Console.WriteLine("Updated Type value: " + binding.Type);
                
                Console.WriteLine("Type property has been successfully demonstrated");
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

* class [WebExtensionBinding](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


