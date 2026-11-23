---
title: "WebExtensionBinding.Appref"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionBinding. Obtient et définit la clé de liaison utilisée pour mapper l'entrée de liaison dans cette liste avec les données liées dans le document"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionbinding/appref/
---
## WebExtensionBinding.Appref property

Obtient et définit la clé de liaison utilisée pour associer l'entrée de liaison dans cette liste aux données liées dans le document.

```csharp
public string Appref { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingPropertyApprefDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle instance de WebExtensionBinding
                WebExtensionBinding binding = new WebExtensionBinding();
                
                // Définir les propriétés incluant Appref
                binding.Id = "Binding1";
                binding.Type = "text";
                binding.Appref = "Sheet1!A1:B2";
                
                // Afficher la valeur actuelle de Appref
                Console.WriteLine("Appref value: " + binding.Appref);
                
                // Modifier la valeur de Appref pour démontrer qu'elle est en lecture/écriture
                binding.Appref = "Sheet1!C3:D4";
                Console.WriteLine("Updated Appref value: " + binding.Appref);
                
                Console.WriteLine("Appref property has been successfully demonstrated");
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


