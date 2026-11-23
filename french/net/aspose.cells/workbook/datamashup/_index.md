---
title: "Workbook.DataMashup"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient les données de mashup"
type: docs
url: /fr/net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Obtient les données mashup.

```csharp
public DataMashup DataMashup { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyDataMashupDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple pour déclencher Power Query
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);

            // Enregistrer dans un fichier
            string sourcePath = "source.xlsx";
            workbook.Save(sourcePath);

            // Rouvrir le classeur pour accéder à DataMashup
            workbook = new Workbook(sourcePath);
            
            // Accéder aux formules Power Query via la propriété DataMashup
            var queries = workbook.DataMashup.PowerQueryFormulas;
            
            // Afficher les informations de base sur les requêtes
            Console.WriteLine($"Number of Power Query formulas: {queries.Count}");
            
            // S'il existe des requêtes, afficher les détails de la première
            if (queries.Count > 0)
            {
                foreach (var query in queries)
                {
                    Console.WriteLine($"Query Name: {query.Name}");
                    Console.WriteLine($"Number of items: {query.PowerQueryFormulaItems.Count}");
                    break; // Just show first query for demo
                }
            }

            // Enregistrer dans un nouveau fichier
            string destPath = "output.xlsx";
            workbook.Save(destPath);
        }
    }
}
```

### Voir aussi

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


