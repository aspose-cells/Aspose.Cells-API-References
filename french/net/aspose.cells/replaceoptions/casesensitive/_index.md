---
title: "ReplaceOptions.CaseSensitive"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReplaceOptions. Indique si la chaîne recherchée est sensible à la casse"
type: docs
url: /fr/net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Indique si la chaîne recherchée est sensible à la casse.

```csharp
public bool CaseSensitive { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Créer des options de remplacement avec CaseSensitive = false
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            
            // Remplacer toutes les variantes de casse de \"apple\" par \"orange\"
            workbook.Replace("apple", "orange", options);

            // Afficher les résultats
            Console.WriteLine("After replacement (CaseSensitive = false):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // Réinitialiser les données
            worksheet.Cells["A2"].PutValue("apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("APPLE");

            // Modifier en CaseSensitive = true
            options.CaseSensitive = true;
            workbook.Replace("apple", "orange", options);

            // Afficher les résultats
            Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### Voir aussi

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


