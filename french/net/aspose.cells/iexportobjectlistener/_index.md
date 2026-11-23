---
title: "Interface IExportObjectListener"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Interface Aspose.Cells.IExportObjectListener. Permet aux utilisateurs de manipuler les objets lors de l'exportation"
type: docs
url: /fr/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Permet aux utilisateurs de manipuler les objets lors de l'exportation.

```csharp
public interface IExportObjectListener
```

## Méthodes

| Nom | Description |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Exporter un objet. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassIExportObjectListenerDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une image d'exemple à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Implémentation personnalisée du listener d'exportation
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // Enregistrer en HTML avec un listener personnalisé
            workbook.Save("output.html", saveOptions);
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        
        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                if (shape.MsoDrawingType == MsoDrawingType.Picture)
                {
                    string url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                    imgIdx++;
                    return url;
                }
            }
            return null;
        }
        
        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // Dans une implémentation réelle, vous enregistreriez l'image sur le disque ici
            // À des fins de démonstration, nous renvoyons simplement un chemin factice
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


