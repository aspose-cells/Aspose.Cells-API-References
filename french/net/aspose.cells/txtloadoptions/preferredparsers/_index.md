---
title: "TxtLoadOptions.PreferredParsers"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété TxtLoadOptions. Obtient et définit les analyseurs de valeurs préférés pour le chargement d'un fichier texte"
type: docs
url: /fr/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Obtient et définit les analyseurs de valeurs préférés pour le chargement d'un fichier texte.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Remarques

parsers[0] est l'analyseur qui sera utilisé pour la première colonne du fichier modèle texte, parsers[1] est l'analyseur qui sera utilisé pour la deuxième colonne, ...etc. Le dernier (parsers[parsers.length-1]) sera utilisé pour toutes les autres colonnes à partir de parsers.length-1. Si un élément est nul, la colonne correspondante sera analysée par l'analyseur par défaut d'Aspose.Cells.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // Créer des options de chargement CSV
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // Définir les analyseurs préférés - d'abord essayer l'analyseur de chaîne personnalisé, puis les analyseurs par défaut
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // Exemple de données CSV avec des dates
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // Charger le classeur avec des options
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // Vérifier les résultats de l'analyse
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### Voir aussi

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


