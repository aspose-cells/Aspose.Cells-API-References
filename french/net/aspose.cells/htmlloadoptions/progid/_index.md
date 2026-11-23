---
title: "HtmlLoadOptions.ProgId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlLoadOptions. Obtient l'identifiant du programme qui crée le fichier. Seulement pour les fichiers MHT"
type: docs
url: /fr/net/aspose.cells/htmlloadoptions/progid/
---
## HtmlLoadOptions.ProgId property

Obtient l'identifiant du programme qui crée le fichier. Uniquement pour les fichiers MHT.

```csharp
public string ProgId { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyProgIdDemo
    {
        public static void Run()
        {
            // Créer des options de chargement HTML au format MHTML
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.MHtml);
            
            // Obtenir la propriété ProgId
            Console.WriteLine("ProgId is: " + options.ProgId);

            // Créer une autre instance et obtenir son ProgId
            HtmlLoadOptions wordOptions = new HtmlLoadOptions(LoadFormat.MHtml);
            Console.WriteLine("ProgId is: " + wordOptions.ProgId);
        }
    }
}
```

### Voir aussi

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


