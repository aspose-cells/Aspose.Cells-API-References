---
title: "Interface IStreamProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.IStreamProvider. Représente le fournisseur de flux exporté"
type: docs
url: /fr/net/aspose.cells/istreamprovider/
---
## IStreamProvider interface

Représente le fournisseur de flux exporté.

```csharp
public interface IStreamProvider
```

## Méthodes

| Nom | Description |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Ferme le flux. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Obtient le flux. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class IStreamProviderDemo : IStreamProvider
    {
        // Implémentation de la méthode InitStream
        public void InitStream(StreamProviderOptions options)
        {
            string outputDir = "/test/";
            string path = outputDir + Path.GetFileName(options.DefaultPath);
            options.CustomPath = path;
            Directory.CreateDirectory(Path.GetDirectoryName(path));
            options.Stream = File.Create(path);
        }

        // Implémentation de la méthode CloseStream
        public void CloseStream(StreamProviderOptions options)
        {
            // Fermez le flux s'il n'est pas nul
            if (options.Stream != null)
            {
                options.Stream.Close();
            }
        }

        public static void IStreamProviderExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définissez certaines données dans la feuille de calcul
            worksheet.Cells["A1"].PutValue("Hello World");

            // Créer HtmlSaveOptions et définir le StreamProvider
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new IStreamProviderDemo();

            // Enregistrer le classeur au format HTML
            workbook.Save("IStreamProviderExample.html", saveOptions);

            // Charger le classeur depuis le format HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new IStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);

            // Afficher les données chargées
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }

}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


