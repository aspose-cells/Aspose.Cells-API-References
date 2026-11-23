---
title: "ReferredArea.ExternalFileName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReferredArea property. Obtenez le nom de fichier externe si c'est une référence externe"
type: docs
url: /fr/net/aspose.cells/referredarea/externalfilename/
---
## ReferredArea.ExternalFileName property

Obtenir le nom du fichier externe si c'est une référence externe.

```csharp
public string ExternalFileName { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyExternalFileNameDemo
    {
        public static void Run()
        {
            // Créez un classeur avec une référence externe
            Workbook wb = new Workbook();
            
            // Créez un nom qui fait référence à un classeur externe
            int index = wb.Worksheets.Names.Add("RefExternalName");
            wb.Worksheets.Names[index].RefersTo = "='[ExternalLinkSource.xlsx]Sheet1'!$A$1:$C$3";
            
            // Obtenez la zone référencée
            ReferredArea ra = wb.Worksheets.Names["RefExternalName"].GetReferredAreas(false)[0];
            
            // Démontrez la propriété ExternalFileName
            Console.WriteLine("External File Name: " + ra.ExternalFileName);
            Console.WriteLine("Sheet Name: " + ra.SheetName);
            Console.WriteLine("Area: R" + ra.StartRow + "C" + ra.StartColumn + 
                              " to R" + ra.EndRow + "C" + ra.EndColumn);
            
            // Vérifiez le nom de fichier externe
            if (!ra.ExternalFileName.EndsWith("ExternalLinkSource.xlsx"))
            {
                Console.WriteLine("Error: ExternalFileName should be ExternalLinkSource.xlsx");
            }
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


