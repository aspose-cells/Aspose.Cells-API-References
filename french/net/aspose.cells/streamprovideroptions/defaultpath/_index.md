---
title: "StreamProviderOptions.DefaultPath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StreamProviderOptions. L'URL du chemin par défaut enregistrée dans le fichier HTML généré pour la source référencée. Par exemple, les données de la feuille enregistrées dans xxx_files/sheet001.htm, l'URL utilisée dans le fichier HTML principal devrait être comme srcxxx_files/sheet001.htm"
type: docs
url: /fr/net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

Le chemin par défaut (URL) enregistré dans le fichier HTML généré pour la source référencée. Par exemple, les données de la feuille enregistrées dans xxx_files/sheet001.htm, l'URL utilisée dans le fichier HTML principal devrait être comme "src=\"xxx_files/sheet001.htm\""

```csharp
public string DefaultPath { get; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyDefaultPathDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer StreamProviderOptions avec ResourceLoadingType et DefaultPath
            StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
            
            // Démontrer l'utilisation de DefaultPath
            Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
            
            // Exemple d'utilisation des options avec un flux (démo simplifiée)
            using (MemoryStream stream = new MemoryStream())
            {
                options.Stream = stream;
                
                if (options.DefaultPath.IndexOf("1.") >= 0)
                {
                    Console.WriteLine("Processing stream for path: " + options.DefaultPath);
                    // Effectuer des opérations avec le flux
                    workbook.Save(stream, SaveFormat.Xlsx);
                }
            }
        }
    }
}
```

### Voir aussi

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


