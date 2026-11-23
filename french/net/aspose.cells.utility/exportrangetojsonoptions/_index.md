---
title: "Classe ExportRangeToJsonOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Utility.ExportRangeToJsonOptions. Indique les options d'exportation de la plage vers JSON"
type: docs
url: /fr/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Indique les options d'exportation d'une plage vers JSON.

```csharp
public class ExportRangeToJsonOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Exporte la valeur chaîne des cellules vers JSON. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Indique s’il faut exporter les cellules vides en tant que null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Indique si la plage contient une ligne d'en-tête. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Indique l’indentation. |

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple aux cellules
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créez des options d'exportation
            var exportOptions = new ExportRangeToJsonOptions();
            
            // Exportez la plage vers JSON
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // Générez le JSON
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // Enregistrez dans un fichier (optionnel)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


