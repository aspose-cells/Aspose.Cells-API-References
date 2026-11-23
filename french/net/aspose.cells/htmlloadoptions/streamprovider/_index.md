---
title: "HtmlLoadOptions.StreamProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Obtient ou définit le StreamProviderImportHtmlFile pour l'importation d'objets"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/streamprovider/
---
## HtmlLoadOptions.StreamProvider property

Obtient ou définit le StreamProviderImportHtmlFile pour l'importation d'objets.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyStreamProviderDemo : IStreamProvider
    {
        public void InitStream(StreamProviderOptions options)
        {
            // Initialisez le flux selon les besoins
        }

        public Stream ProvideStream(StreamProviderOptions options)
        {
            // Renvoie un flux pour la lecture/écriture
            return File.Open(options.DefaultPath, FileMode.OpenOrCreate, FileAccess.ReadWrite);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Fermez le flux
            options.Stream.Close();
        }

        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("StreamProvider Demo");

            // Enregistrez avec un StreamProvider personnalisé
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            workbook.Save("output.html", saveOptions);

            // Chargez avec un StreamProvider personnalisé
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            loadOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
            Workbook loadedWorkbook = new Workbook("output.html", loadOptions);

            // Vérifiez les données chargées
            Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Voir aussi

* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


