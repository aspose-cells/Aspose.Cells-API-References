---
title: "Classe ExportObjectEvent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.ExportObjectEvent class. L'événement déclenché lors de l'exportation d'un objet tel que Picture"
type: docs
url: /fr/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

L'événement déclenché lors de l'exportation d'un objet, tel que Picture.

```csharp
public class ExportObjectEvent
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Obtient l'objet à exporter. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventDemo
    {
        public static void ExportObjectEventExample()
        {
            // Implémentation personnalisée de IExportObjectListener
            // Enregistrer le fichier HTML avec un écouteur personnalisé
            Workbook workbook = new Workbook(); // Build your workbook here
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = new CustomExportObjectListener()
            };
            using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
            {
                workbook.Save(stream, saveOptions); // Save the workbook to stream
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;

        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape shape)
            {
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                        break;
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }

        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // Ici, enregistrez l'image à n'importe quel emplacement, puis renvoyez l'URL (relative ou absolue) que le HTML généré peut utiliser pour obtenir l'image
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


