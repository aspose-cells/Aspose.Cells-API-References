---
title: "ExportRangeToJsonOptions.ExportAsString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExportRangeToJsonOptions. Exporte la valeur sous forme de chaîne des cellules au format JSON"
type: docs
url: /fr/net/aspose.cells.utility/exportrangetojsonoptions/exportasstring/
---
## ExportRangeToJsonOptions.ExportAsString property

Exporte la valeur chaîne des cellules vers JSON.

```csharp
public bool ExportAsString { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Remplir les cellules avec différents types de données
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("String");
            worksheet.Cells["B2"].PutValue("Hello");
            worksheet.Cells["A3"].PutValue("Number");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["B4"].PutValue(DateTime.Now);

            // Créer une instance ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Afficher la valeur actuelle de ExportAsString
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Exporter sans ExportAsString (comportement par défaut)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
            string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);

            // Définir ExportAsString sur vrai
            options.ExportAsString = true;

            // Exporter avec ExportAsString
            string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);

            // Enregistrez le classeur
            workbook.Save("ExportAsStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


