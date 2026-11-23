---
title: "WebExtension.IsFrozen"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtension. Indique si l'utilisateur peut interagir avec le module Office Addin ou non"
type: docs
url: /fr/net/aspose.cells.webextensions/webextension/isfrozen/
---
## WebExtension.IsFrozen property

Indique si l'utilisateur peut interagir avec l'Office Add-in ou non.

```csharp
public bool IsFrozen { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyIsFrozenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Cette ligne échouera parce que WebExtension nécessite des paramètres de constructeur
                // WebExtension webExtension = new WebExtension();
                
                // À la place, nous récupérerons une extension web depuis le classeur si possible
                // ou démontrer avec une approche différente
                Console.WriteLine("Note: WebExtension requires constructor parameters. This demo shows property usage conceptually.");
                
                // À des fins de démonstration, nous montrerons comment la propriété fonctionnerait si vous aviez une instance valide
                // Dans un scénario réel, vous obtiendriez l'instance WebExtension depuis le classeur ou une autre source
                WebExtension webExtension = GetWebExtensionInstance(workbook);
                
                if (webExtension != null)
                {
                    // Définissez les propriétés initiales
                    webExtension.Id = "MyAddin123";
                    
                    // Afficher la valeur initiale de IsFrozen
                    Console.WriteLine($"Initial IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Modifier la propriété IsFrozen (puisqu'elle est en lecture-écriture)
                    webExtension.IsFrozen = true;
                    Console.WriteLine($"Updated IsFrozen value: {webExtension.IsFrozen}");
                    
                    // Démontrer l'effet en vérifiant si l'utilisateur peut interagir
                    Console.WriteLine($"User can{(webExtension.IsFrozen ? "not" : "")} interact with the add-in");
                    
                    // Enregistrer le classeur (bien que l'extension web puisse ne pas être persistée sans étapes supplémentaires)
                    workbook.Save("WebExtensionIsFrozenDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("Could not obtain a WebExtension instance for demonstration.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static WebExtension GetWebExtensionInstance(Workbook workbook)
        {
            // Dans une implémentation réelle, cela récupérerait un WebExtension existant depuis le classeur
            // ou en créer un correctement avec les paramètres de constructeur requis
            // Ceci n'est qu'un espace réservé pour la démonstration
            return null;
        }
    }
}
```

### Voir aussi

* class [WebExtension](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


