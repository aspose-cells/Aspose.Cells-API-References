---
title: "TxtLoadOptions.IsMultiEncoded"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Vrai signifie que le fichier contient plusieurs encodages"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/ismultiencoded/
---
## TxtLoadOptions.IsMultiEncoded property

True signifie que le fichier contient plusieurs encodages.

```csharp
public bool IsMultiEncoded { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyIsMultiEncodedDemo
    {
        public static void Run()
        {
            // Créer des options de chargement de texte
            TxtLoadOptions options = new TxtLoadOptions();
            
            // Définissez IsMultiEncoded sur true pour gérer plusieurs encodages
            options.IsMultiEncoded = true;
            
            // Chargez le classeur avec les options
            Workbook workbook = new Workbook("example.csv", options);
            
            // Affichez des valeurs d'exemple du fichier chargé
            Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
            Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
        }
    }
}
```

### Voir aussi

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


