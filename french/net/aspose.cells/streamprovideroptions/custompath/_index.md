---
title: "StreamProviderOptions.CustomPath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StreamProviderOptions. Le pathURL personnalisé de l'utilisateur enregistré dans le fichier HTML généré pour la source référencée. Si l'utilisateur ne le définit pas, DefaultPath sera utilisé. Par exemple, les données de la feuille seront enregistrées par l'utilisateur sous d/sheet001.htm ; l'URL utilisée dans le fichier HTML principal doit être d/sheet001.htm ou tout autre chemin relatif valide pouvant être accédé par le fichier HTML principal."
type: docs
url: /fr/net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

Le chemin personnalisé (URL) de l'utilisateur enregistré dans le fichier HTML généré pour la source référencée. Si l'utilisateur ne le définit pas, DefaultPath sera utilisé. Par exemple, les données de la feuille seront enregistrées par l'utilisateur sous d:/sheet001.htm, l'URL utilisée dans le fichier HTML principal doit être "d:/sheet001.htm" ou tout autre chemin relatif valide pouvant être accédé par le fichier HTML principal.

```csharp
public string CustomPath { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StreamProviderOptionsPropertyCustomPathDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Configurer les options d'enregistrement HTML avec un fournisseur de flux personnalisé
            string outputDir = "output";
            Directory.CreateDirectory(outputDir);
            
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
            
            // Créer un fournisseur de flux personnalisé avec CustomPath
            HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
            streamProvider.streamProviderOptions.CustomPath = "resources";
            options.StreamProvider = streamProvider;

            // Enregistrez le classeur
            string outputFile = Path.Combine(outputDir, "output.html");
            workbook.Save(outputFile, options);

            // Vérifier que le chemin personnalisé a été utilisé
            string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
            Console.WriteLine($"Resources should be saved to: {resourcePath}");
        }
    }

    // Implémentation simplifiée du fournisseur de flux personnalisé
    public class HtmlWithExternalResourcesProvider : IStreamProvider
    {
        public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
        public string _outputDirectory;

        public HtmlWithExternalResourcesProvider(string outputDirectory)
        {
            _outputDirectory = outputDirectory;
        }

        public void InitStream(StreamProviderOptions options)
        {
            // L'implémentation serait placée ici
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // L'implémentation serait placée ici
        }
    }
}
```

### Voir aussi

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


