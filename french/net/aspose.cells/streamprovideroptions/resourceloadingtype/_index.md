---
title: "StreamProviderOptions.ResourceLoadingType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StreamProviderOptions. Obtient et définit le type de chargement de la ressource"
type: docs
url: /fr/net/aspose.cells/streamprovideroptions/resourceloadingtype/
---
## StreamProviderOptions.ResourceLoadingType property

Obtient et définit le type de ressource de chargement.

```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyResourceLoadingTypeDemo
    {
        public static void Run()
        {
            // Créer un classeur avec les options du fournisseur de flux
            var options = new StreamProviderOptions
            {
                ResourceLoadingType = ResourceLoadingType.UserProvided
            };

            // Démontrer différents comportements de chargement de ressources
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Fournir un flux mémoire personnalisé
                options.Stream = new MemoryStream();
                Console.WriteLine("Using user-provided memory stream");
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Ignorer le chargement en utilisant un flux nul
                options.Stream = Stream.Null;
                Console.WriteLine("Skipping resource loading");
            }
            else
            {
                // Comportement de chargement de fichier par défaut
                string defaultPath = "default_resource.txt";
                options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
                Console.WriteLine("Loading resource from default path");
            }

            // Nettoyage
            options.Stream?.Dispose();
        }
    }
}
```

### Voir aussi

* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


