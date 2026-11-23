---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit l'ExportObjectListener pour l'exportation d'objets"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Obtient ou définit l'ExportObjectListener pour l'exportation d'objets.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété HtmlSaveOptions.IStreamProvider. Cette propriété sera supprimée 12 mois plus tard, depuis août 2015. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportObjectListenerDemo
    {
        public static void Run()
        {
            // Créer un écouteur d'exportation d'objet personnalisé
            var listener = new CustomExportObjectListener();
            
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // Créer des options d'enregistrement HTML avec l'écouteur
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // Enregistrer dans un fichier HTML
            workbook.Save("output.html", saveOptions);
        }
    }

    // Implémentation personnalisée de IExportObjectListener
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Exemple : traiter l'objet exporté
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // Retourner l'objet original (peut le modifier si nécessaire)
            return e;
        }
    }
}
```

### Voir aussi

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


