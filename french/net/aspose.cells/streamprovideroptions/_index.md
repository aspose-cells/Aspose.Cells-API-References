---
title: "Classe StreamProviderOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.StreamProviderOptions. Représente les options de flux"
type: docs
url: /fr/net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Représente les options de flux.

```csharp
public class StreamProviderOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Initialise une nouvelle instance de la classe `StreamProviderOptions`. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Initialise une nouvelle instance de la classe `StreamProviderOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | Le chemin personnalisé (URL) de l'utilisateur enregistré dans le fichier HTML généré pour la source référencée. Si l'utilisateur ne le définit pas, DefaultPath sera utilisé. Par exemple, les données de la feuille seront enregistrées par l'utilisateur sous d:/sheet001.htm, l'URL utilisée dans le fichier HTML principal doit être "d:/sheet001.htm" ou tout autre chemin relatif valide pouvant être accédé par le fichier HTML principal. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | Le chemin par défaut (URL) enregistré dans le fichier HTML généré pour la source référencée. Par exemple, les données de la feuille enregistrées dans xxx_files/sheet001.htm, l'URL utilisée dans le fichier HTML principal devrait être comme "src=\"xxx_files/sheet001.htm\"" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Obtient et définit le type de ressource de chargement. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Obtient/Définit le flux |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassStreamProviderOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer StreamProviderOptions
            StreamProviderOptions options = new StreamProviderOptions();
            
            // Définir un flux mémoire pour la démonstration
            options.Stream = new MemoryStream();
            
            // Utiliser le flux (exemple : enregistrer le classeur dans le flux)
            workbook.Save(options.Stream, SaveFormat.Xlsx);
            
            // Démontrer la fermeture du flux
            CloseStream(options);
        }

        public static void CloseStream(StreamProviderOptions options)
        {
            if (options.Stream != null)
            {
                options.Stream.Close();
                options.Stream = null;
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


