---
title: "JsonSaveOptions.HasHeaderRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Indique si la plage contient une ligne d'en-tête"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/hasheaderrow/
---
## JsonSaveOptions.HasHeaderRow property

Indique si la plage contient une ligne d'en-tête.

```csharp
public bool HasHeaderRow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyHasHeaderRowDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une ligne d'en-tête
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            
            // Ajouter des lignes de données
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer une plage (A1:B3)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);

            // Exporter en JSON avec HasHeaderRow = true (par défaut)
            JsonSaveOptions options1 = new JsonSaveOptions();
            options1.HasHeaderRow = true;
            string jsonWithHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options1);
            Console.WriteLine("JSON with headers:\n" + jsonWithHeaders);

            // Exporter en JSON avec HasHeaderRow = false
            JsonSaveOptions options2 = new JsonSaveOptions();
            options2.HasHeaderRow = false;
            string jsonWithoutHeaders = Aspose.Cells.Utility.JsonUtility.ExportRangeToJson(range, options2);
            Console.WriteLine("\nJSON without headers:\n" + jsonWithoutHeaders);
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


