---
title: "ExportObjectEvent.GetSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ExportObjectEvent. Obtient l'objet à exporter"
type: docs
url: /fr/net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Obtient l'objet à exporter.

```csharp
public object GetSource()
```

### Valeur de retour

l'objet à exporter.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventMethodGetSourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image pour démontrer la fonctionnalité GetSource
            int pictureIndex = worksheet.Pictures.Add(1, 1, "sample.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            try
            {
                // Créer un écouteur d'exportation d'objet personnalisé
                HtmlSaveOptions saveOptions = new HtmlSaveOptions
                {
                    ExportObjectListener = new CustomExportObjectListener()
                };

                // Enregistrer le classeur pour déclencher l'événement ExportObjectEvent
                using (Stream stream = new FileStream("GetSourceDemo.html", FileMode.Create))
                {
                    workbook.Save(stream, saveOptions);
                }

                Console.WriteLine("GetSource method demonstrated successfully. Check the output HTML file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetSource: {ex.Message}");
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Démontrer la méthode GetSource
            object source = e.GetSource();

            if (source is Picture)
            {
                Console.WriteLine("GetSource returned a Picture object");
                return "custom-image-url.jpg";
            }

            return null;
        }
    }
}
```

### Voir aussi

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


