---
title: "PageSetup.GetHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Obtient un script formatant l'en-tête d'un fichier Excel"
type: docs
url: /fr/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Obtient un script formatant l'en-tête d'un fichier Excel.

```csharp
public string GetHeader(int section)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir l'en-tête pour la section 2
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // Récupérez et imprimez l'en-tête pour la section 2
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


