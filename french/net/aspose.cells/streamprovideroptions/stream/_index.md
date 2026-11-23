---
title: "StreamProviderOptions.Stream"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StreamProviderOptions. Obtient/ Définit le flux"
type: docs
url: /fr/net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Obtient/Définit le flux

```csharp
public Stream Stream { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyStreamDemo
    {
        public static void Run()
        {
            // Créer une instance de StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Cas 1 : lorsqu'aucun chemin par défaut n'est défini – utilisez MemoryStream
            options.Stream = new MemoryStream();
            Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));

            // Cas 2 : simuler la présence d'un chemin par défaut – utilisez FileStream
            string outputDir = "output/";
            string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
            string path = outputDir + Path.GetFileName(defaultPath);
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
            Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
            
            // Nettoyer
            options.Stream.Dispose();
            if (File.Exists(path))
            {
                File.Delete(path);
            }
        }
    }
}
```

### Voir aussi

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


