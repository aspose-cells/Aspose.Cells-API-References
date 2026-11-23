---
title: "ExternalLinkCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ExternalLinkCollection. Obtient un énumérateur qui parcourt cette collection"
type: docs
url: /fr/net/aspose.cells/externallinkcollection/getenumerator/
---
## ExternalLinkCollection.GetEnumerator method

Obtenez un énumérateur qui parcourt cette collection.

```csharp
public IEnumerator GetEnumerator()
```

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez quelques liens externes en utilisant la signature correcte de la méthode Add
            workbook.Worksheets.ExternalLinks.Add("externallink1.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink2.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink3.xlam", new string[] { "Sheet1!A1" });
            workbook.Worksheets.ExternalLinks.Add("externallink4.xlam", new string[] { "Sheet1!A1" });

            // Obtenez la ExternalLinkCollection
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            
            // Démontrez l'utilisation de GetEnumerator
            Console.WriteLine("Enumerating external links:");
            IEnumerator enumerator = externalLinks.GetEnumerator();
            int count = 0;
            while (enumerator.MoveNext())
            {
                ExternalLink link = (ExternalLink)enumerator.Current;
                Console.WriteLine($"{++count}. {link.DataSource}");
            }

            // Ajoutez des formules faisant référence à ces liens externes
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                worksheet.Cells[i, 0].Formula = $"=externallink{i+1}.xlam!customfunc()";
            }

            Console.WriteLine("\nFormulas referencing external links:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {worksheet.Cells[i, 0].Formula}");
            }
        }
    }
}
```

### Voir aussi

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


