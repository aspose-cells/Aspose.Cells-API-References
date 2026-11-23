---
title: "Workbook.HasExernalLinks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Indique si ce classeur contient des liens externes vers d’autres sources de données"
type: docs
url: /fr/net/aspose.cells/workbook/hasexernallinks/
---
## Workbook.HasExernalLinks method

Indique si ce classeur contient des liens externes vers d’autres sources de données.

```csharp
[Obsolete("Use ExternalLinkCollection.Count property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasExernalLinks()
```

### Valeur de retour

Si ce classeur contient des liens externes vers d’autres sources de données.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser ExternalLinkCollection.Count pour vérifier s’il existe des liens externes dans ce classeur. Cette méthode sera supprimée 12 mois après décembre 2021. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodHasExernalLinksDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des liens externes
            var workbook = new Workbook();
            var worksheet = workbook.Worksheets[0];
            
            // Ajouter un lien externe
            worksheet.Cells["A1"].Formula = "='http://example.com/[external.xlsx]Sheet1'!A1";
            
            // Vérifier si le classeur possède des liens externes
            if (workbook.HasExernalLinks())
            {
                Console.WriteLine("Workbook contains external links:");
                foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
                {
                    Console.WriteLine($"External Link: {link.DataSource}");
                }
            }
            else
            {
                Console.WriteLine("Workbook has no external links");
            }
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


