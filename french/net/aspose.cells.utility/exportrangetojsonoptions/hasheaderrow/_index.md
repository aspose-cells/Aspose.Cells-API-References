---
title: "ExportRangeToJsonOptions.HasHeaderRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportRangeToJsonOptions. Indique si la plage contient une ligne d’en-tête"
type: docs
url: /fr/net/aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/
---
## ExportRangeToJsonOptions.HasHeaderRow property

Indique si la plage contient une ligne d'en-tête.

```csharp
public bool HasHeaderRow { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les données d'exemple avec les en-têtes
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Créer la plage à exporter
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");

            // Créer une instance ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();

            // Afficher la valeur actuelle de HasHeaderRow (false par défaut)
            Console.WriteLine("Current HasHeaderRow value: " + options.HasHeaderRow);

            // Définir HasHeaderRow sur vrai
            options.HasHeaderRow = true;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exporter vers JSON avec les en-têtes
            string jsonWithHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Définir HasHeaderRow sur faux
            options.HasHeaderRow = false;
            Console.WriteLine("New HasHeaderRow value: " + options.HasHeaderRow);

            // Exporter vers JSON sans les en-têtes
            string jsonWithoutHeaders = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without headers:\n" + jsonWithoutHeaders);

            // Enregistrez le classeur
            workbook.Save("PropertyHasHeaderRowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


