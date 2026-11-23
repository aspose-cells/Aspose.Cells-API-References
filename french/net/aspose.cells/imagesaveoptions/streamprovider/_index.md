---
title: "ImageSaveOptions.StreamProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImageSaveOptions. Obtient ou définit l'IStreamProvider pour l'exportation d'objets"
type: docs
url: /fr/net/aspose.cells/imagesaveoptions/streamprovider/
---
## ImageSaveOptions.StreamProvider property

Obtient ou définit le IStreamProvider pour l'exportation d'objets.

```csharp
public IStreamProvider StreamProvider { get; set; }
```

### Remarques

Si l'enregistrement se fait au format Tiff, cette propriété est ignorée. Sinon, si plusieurs images doivent être enregistrées, nous écrirons les autres images à l'aide de celle-ci. Pour une utilisation avancée, veuillez utiliser [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) ou [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomStreamProvider : IStreamProvider
    {
        private int m_count = 0;

        public void InitStream(StreamProviderOptions options)
        {
            m_count++;
        }

        public Stream GetStream(StreamProviderOptions options)
        {
            return new FileStream(options.DefaultPath + m_count + ".png", FileMode.Create);
        }

        public void CloseStream(StreamProviderOptions options)
        {
            // Implémentation lorsqu'aucun flux n'est fourni
        }

        public void CloseStream(StreamProviderOptions options, Stream stream)
        {
            stream.Dispose();
        }
    }

    public class ImageSaveOptionsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test StreamProvider");

            // Définir les options d'enregistrement avec un fournisseur de flux personnalisé
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            saveOptions.StreamProvider = new CustomStreamProvider();

            // Enregistrer avec le fournisseur de flux
            workbook.Save("output.png", saveOptions);
        }
    }
}
```

### Voir aussi

* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


