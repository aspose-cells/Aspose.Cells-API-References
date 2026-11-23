---
title: "WebExtensionBinding.Id"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionBinding. Obtient et définit l'identifiant de liaison"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionbinding/id/
---
## WebExtensionBinding.Id property

Obtient et définit l'identifiant de liaison.

```csharp
public string Id { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyIdDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle instance de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Définir la propriété Id
                binding.Id = "SampleBindingId";
                
                // Afficher la valeur actuelle de Id
                Console.WriteLine("Initial Id value: " + binding.Id);
                
                // Modifier la valeur de Id pour démontrer qu'elle est en lecture/écriture
                binding.Id = "UpdatedBindingId";
                Console.WriteLine("Updated Id value: " + binding.Id);
                
                Console.WriteLine("Id property has been successfully demonstrated");
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


