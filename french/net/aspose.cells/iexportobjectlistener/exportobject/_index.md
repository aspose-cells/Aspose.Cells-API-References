---
title: "IExportObjectListener.ExportObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode IExportObjectListener. Exporter un objet"
type: docs
url: /fr/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

Exporter un objet.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| e | ExportObjectEvent | L'événement déclenché lorsqu'un objet doit être exporté. |

### Valeur de retour

Les informations sur le résultat de l'exportation d'un objet. Lors de l'exportation d'objets lors de l'exportation du classeur au format HTML, le résultat est une chaîne URL permettant d'accéder à l'image enregistrée depuis le fichier HTML qui contient cet objet exporté.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une image à la feuille de calcul
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Créer une instance de la classe de démonstration implémentant IExportObjectListener
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // Dans un scénario réel, l'ExportObjectEvent serait fourni par le framework
                // À des fins de démonstration, nous appellerons simplement la méthode avec null
                object result = listener.ExportObject(null);

                Console.WriteLine("ExportObject method executed successfully.");
                Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
            }

            workbook.Save("ExportObjectDemo.xlsx");
        }

        public object ExportObject(ExportObjectEvent e)
        {
            // Implémentation personnalisée pour gérer l'exportation
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // Retourner un objet modifié ou null pour utiliser le comportement d'exportation par défaut
            return null;
        }
    }
}
```

### Voir aussi

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


