---
title: "ReplaceOptions.RegexKey"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ReplaceOptions. Indique si la clé recherchée est une expression régulière. Si vrai, la clé recherchée sera considérée comme une expression régulière"
type: docs
url: /fr/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Indique si la clé recherchée est une expression régulière. Si true, la clé recherchée sera prise comme expression régulière.

```csharp
public bool RegexKey { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // Créer des options de remplacement avec regex
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // Remplacer tous les mots commençant par 'p' ou 'b' suivis d'une voyelle
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // Effectuer le remplacement
            workbook.Replace(pattern, replacement, options);

            // Enregistrer le résultat
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


