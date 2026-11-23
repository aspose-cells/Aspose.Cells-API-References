---
title: "PasteOptions.IgnoreLinksToOriginalFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PasteOptions. Ignorer les liens vers le fichier original"
type: docs
url: /fr/net/aspose.cells/pasteoptions/ignorelinkstooriginalfile/
---
## PasteOptions.IgnoreLinksToOriginalFile property

Ignorer les liens vers le fichier original.

```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet src = workbook.Worksheets[0];
            
            // Créer des données d'exemple avec des formules pouvant être liées au fichier original
            src.Cells["A1"].PutValue("Header1");
            src.Cells["B1"].PutValue("Header2");
            src.Cells["A2"].PutValue(100);
            src.Cells["B2"].PutValue("=A2*2");  // Simple formula
            src.Cells["A3"].PutValue(200);
            src.Cells["B3"].PutValue("=A3*2");

            // Créer la feuille de destination et la plage
            Worksheet dst = workbook.Worksheets.Add("Destination");
            Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");

            // Configurer les options de collage pour ignorer les liens vers le fichier original
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.PasteType = PasteType.All;
            pasteOptions.IgnoreLinksToOriginalFile = true;

            // Copier avec les options de collage spécifiées
            dstRange.Copy(srcRange, pasteOptions);

            // Enregistrez le classeur
            workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


