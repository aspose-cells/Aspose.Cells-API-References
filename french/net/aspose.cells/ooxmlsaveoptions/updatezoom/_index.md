---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OoxmlSaveOptions. Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent la mise à l'échelle de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

Indique s'il faut mettre à jour le facteur d'échelle avant d'enregistrer le fichier si les propriétés PageSetup.FitToPagesWide et PageSetup.FitToPagesTall contrôlent la mise à l'échelle de la feuille de calcul.

```csharp
public bool UpdateZoom { get; set; }
```

### Remarques

La valeur par défaut est false pour les performances.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyUpdateZoomDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir le niveau de zoom initial
            worksheet.PageSetup.Zoom = 100;

            // Créer des options d'enregistrement avec UpdateZoom activé
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // Enregistrer dans le flux mémoire
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Recharger le classeur pour vérifier que le zoom a été mis à jour
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### Voir aussi

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


