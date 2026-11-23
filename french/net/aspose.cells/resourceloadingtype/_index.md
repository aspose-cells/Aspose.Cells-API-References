---
title: "Enum ResourceLoadingType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ResourceLoadingType enum. Représente comment charger la ressource liée"
type: docs
url: /fr/net/aspose.cells/resourceloadingtype/
---
## ResourceLoadingType enumeration

Représente la façon de charger la ressource liée.

```csharp
public enum ResourceLoadingType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Default | `0` | Charge cette ressource comme d'habitude. |
| Skip | `1` | Ignore le chargement de cette ressource. |
| UserProvided | `2` | Utilisez le flux fourni par l'utilisateur |

### Exemples

```csharp
using Aspose.Cells;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ResourceLoadingTypeDemo
    {
        public static void ResourceLoadingTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Resource");
            worksheet.Cells["A2"].PutValue("Default");
            worksheet.Cells["A3"].PutValue("Skip");
            worksheet.Cells["A4"].PutValue("UserProvided");

            // Enregistrez le classeur au format HTML avec un fournisseur de flux personnalisé
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                StreamProvider = new CustomStreamProvider()
            };

            workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
        }
    }

    public class CustomStreamProvider : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
            {
                // Fournissez un flux personnalisé pour la ressource
                options.Stream = new MemoryStream();
            }
            else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
            {
                // Ignorer le chargement de la ressource
                options.Stream = Stream.Null;
            }
            else
            {
                // Chargez la ressource comme d'habitude
                options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
            }
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Fermez le flux s'il n'est pas nul
            options.Stream?.Close();
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


